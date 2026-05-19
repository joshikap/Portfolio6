---
layout: post
title: Instantiation & Objects in My Game
permalink: /instantiation-objects/
description: How instantiation and objects are used in my JavaScript ocean game.
---

# Instantiation & Objects in My Game

## What Is Instantiation?

Instantiation is the process of creating an object from a class.

A class is a blueprint, while an object is the actual usable item created from that blueprint.

Objects allow the game to create:
- players
- enemies
- NPCs
- score systems
- backgrounds

---

# What Are Objects?

Objects contain:
- properties
- variables
- methods
- behaviors

In my game, objects represent things that exist in the game world.

For example:
- the octopus player
- sharks
- enemies
- coins
- the scoreboard

---

# Example 1: Creating a GameScorer Object

One example of instantiation in my game is:

```javascript
gameEnv.gameScorer = new GameScorer(gameEnv);
```

## Explanation

This line:
1. creates a new object from the `GameScorer` class
2. stores it inside the game environment
3. allows the game to track score and coins

The keyword:

```javascript
new
```

is used to instantiate objects.

---

# Example 2: Creating the Player Object

The player is also created as an object.

```javascript
{ class: Player, data: octopusData }
```

## Explanation

This creates a player object using the `Player` class.

The object contains:
- player movement
- animations
- collisions
- hitboxes
- controls

This allows the octopus character to function inside the game.

---

# Example 3: Enemy Objects

Multiple enemy objects are created using reusable data.

```javascript
const sprite_data_enemy = {
  ...baseEnemy,
  id: "EnemyElon"
};
```

## Explanation

This creates an enemy object with:
- enemy movement
- collision behavior
- AI tracking
- rendering information

Different enemy objects can reuse the same base system.

---

# Example 4: Shark Object

The shark enemy is also instantiated as an object.

```javascript
{ class: Shark, data: sprite_data_shark }
```

## Explanation

This creates a shark object using the custom `Shark` class.

The shark object:
- follows the player
- updates movement
- interacts with the game world

Objects allow enemies to behave independently.

---

# Example 5: Goldfish Objects

My game creates many goldfish objects using loops.

```javascript
const goldfishList = Array.from({ length: 10 }).map((_, i) => ({
  class: Npc,
  data: {
    id: `Goldfish${i}`
  }
}));
```

## Explanation

This creates multiple goldfish objects automatically.

Each object has:
- its own position
- its own ID
- collectible behavior

Instantiation makes large game systems much easier to build.

---

# Why Instantiation & Objects Are Important

Instantiation and objects helped my project by:
- creating reusable systems
- organizing game entities
- reducing repeated code
- improving scalability
- simplifying game management

Without objects, every game entity would need separate hardcoded logic.