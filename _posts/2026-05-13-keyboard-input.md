---
layout: post
title: Keyboard Input in My Game
permalink: /keyboard-input/
description: How keyboard input is used in my JavaScript ocean game.
---

# Keyboard Input in My Game

## What Is Keyboard Input?

Keyboard input allows a player to control a game using keys on a keyboard.

Games use keyboard input for:
- movement
- actions
- menus
- interactions
- gameplay controls

My game uses keyboard input to control the octopus player.

---

# Why Keyboard Input Is Important

Without keyboard input, the player could not:
- move the character
- interact with the game
- avoid enemies
- collect coins
- control gameplay

Keyboard input makes the game interactive and playable.

---

# Example 1: Player Class

My game uses a Player class that responds to keyboard controls.

```javascript
{ class: Player, data: octopusData }
```

## Explanation

The `Player` object:
- handles movement
- responds to keyboard input
- updates player position

This allows the user to control the octopus.

---

# Example 2: Movement Updates

Keyboard input changes player position.

```javascript
this.position.x += Math.cos(angle) * speed;
```

## Explanation

When movement keys are pressed:
- player position changes
- movement updates continuously
- the character moves across the screen

Input controls movement behavior.

---

# Example 3: Directional Animation

Keyboard input controls player animations.

```javascript
left: { row: 1, start: 0, columns: 2 },
right: { row: 1, start: 0, columns: 2 },
up: { row: 2, start: 0, columns: 2 },
down: { row: 0, start: 0, columns: 2 },
```

## Explanation

Different key presses:
- trigger different animations
- change sprite directions
- update visual movement

This creates responsive gameplay.

---

# Example 4: Updating the Player

The game continuously updates player behavior.

```javascript
update: function () {

}
```

## Explanation

The update system:
- checks keyboard input repeatedly
- updates movement
- handles collisions
- processes gameplay logic

Games constantly listen for player input.

---

# Example 5: Collision Reactions

Keyboard movement affects collisions.

```javascript
if (dist < 40)
```

## Explanation

As the player moves:
- collisions are checked
- enemies react
- score changes occur

Keyboard input directly affects gameplay events.

---

# Example 6: Collecting Goldfish

Player movement allows coin collection.

```javascript
this.gameEnv.gameScorer.collectCoin(10);
```

## Explanation

When the player moves into goldfish:
- the object is collected
- score increases
- feedback appears on screen

Keyboard controls make progression possible.

---

# Example 7: Enemy Avoidance

Keyboard input helps avoid enemies.

```javascript
this.gameEnv.gameScorer.deductPoints(10);
```

## Explanation

Players must:
- move away from enemies
- avoid collisions
- navigate the environment

Keyboard input creates challenge and gameplay strategy.

---

# Example 8: Real-Time Gameplay

Keyboard systems work continuously during the game.

```javascript
ANIMATION_RATE: 100
```

## Explanation

The game constantly:
- listens for input
- updates movement
- refreshes animations

This creates smooth real-time gameplay.

---

# Why Keyboard Input Helps My Game

Keyboard input improved my project by:
- enabling player control
- creating interactive gameplay
- supporting movement systems
- allowing enemy avoidance
- making the game responsive and engaging

Without keyboard input, the player could not interact with the game world.