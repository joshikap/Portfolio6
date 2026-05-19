---
layout: post
title: Conditionals in My Game
permalink: /conditionals/
description: How conditionals are used in my JavaScript ocean game.
---

# Conditionals in My Game

## What Are Conditionals?

Conditionals are statements that allow a program to make decisions.

They run code only when certain conditions are true or false.

The most common conditional is:
- `if` statements
- `else if`
- `else`

---

# Why Conditionals Are Important in Games

Games constantly make decisions, such as:
- Did the player collide with an enemy?
- Is the score below zero?
- Should the enemy attack?
- Did the player collect an item?

Without conditionals, the game would not respond to actions.

---

# Example 1: Collision Detection

My game uses conditionals to detect collisions.

```javascript
if (dist < 40) {
  if (!this.gameEnv.elonHitCooldown) {
    this.gameEnv.gameScorer.deductPoints(10);
  }
}
```

## Explanation

This checks:
- if the player is close enough to an enemy
- if cooldown is active or not
- whether to apply damage

---

# Example 2: Preventing Negative Score

Conditionals keep values valid.

```javascript
if (this.score < 0) {
  this.score = 0;
}
```

## Explanation

This ensures:
- score never goes below zero
- game stays fair and stable

---

# Example 3: Checking Enemy State

Enemies use conditionals to stop actions.

```javascript
if (this.isKilling) return;
```

## Explanation

This prevents:
- updates when enemy is inactive
- unwanted behavior during collisions or death states

---

# Example 4: Finding Goldfish

Conditionals are used inside searches.

```javascript
if (fish) fish.destroy();
```

## Explanation

This checks:
- if the object exists
- then removes it safely
- prevents errors if object is missing

---

# Example 5: Player Targeting Logic

Conditionals help AI make decisions.

```javascript
if (dist < minDist) {
  nearest = player;
  minDist = dist;
}
```

## Explanation

This checks:
- if current player is closer than previous one
- updates the target accordingly

This is used in enemy AI.

---

# Why Conditionals Help My Game

Conditionals improved my project by:
- enabling decision-making in gameplay
- handling collisions and interactions
- controlling enemy behavior
- preventing errors and invalid values
- making the game responsive to player actions

Without conditionals, the game would not be interactive or dynamic.