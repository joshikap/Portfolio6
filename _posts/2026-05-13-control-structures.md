---
layout: post
title: Control Structures in My Game
permalink: /control-structures/
description: How control structures are used in my JavaScript ocean game.
---

# Control Structures in My Game

## What Are Control Structures?

Control structures are statements that control the flow of a program.

They decide:
- what code runs
- when code runs
- how often code runs

The main types include:
- if statements
- loops
- switch-like logic (in some systems)

---

# Why Control Structures Are Important

In games, control structures are used to:
- detect collisions
- control enemy behavior
- manage scoring
- check win/lose conditions
- handle player input

Without control structures, the game would run in a fixed, unresponsive way.

---

# Example 1: Collision Check (if statement)

My game uses `if` statements to detect collisions.

```javascript
if (dist < 40) {
  if (!this.gameEnv.elonHitCooldown) {
    this.gameEnv.gameScorer.deductPoints(10);
  }
}
```

## Explanation

This control structure:
- checks distance between objects
- ensures cooldown is not active
- applies damage (score deduction)

It only runs when conditions are true.

---

# Example 2: Preventing Negative Score

Control structures also prevent invalid values.

```javascript
if (this.score < 0) {
  this.score = 0;
}
```

## Explanation

This ensures:
- score never goes below zero
- game values stay valid

This is a simple decision-making structure.

---

# Example 3: Looping Through Enemies

My game uses loops to check all enemies.

```javascript
for (const enemy of enemies) {
  const dx = enemy.position.x - this.position.x;
}
```

## Explanation

This loop:
- goes through every enemy
- calculates distance to each one
- helps determine which enemy is closest

Loops are essential for managing multiple objects.

---

# Example 4: Finding the Nearest Player

Control structures are used in AI behavior.

```javascript
let nearest = players[0];
let minDist = Infinity;

for (const player of players) {
  if (dist < minDist) {
    nearest = player;
    minDist = dist;
  }
}
```

## Explanation

This logic:
- compares distances
- finds closest player
- updates enemy target

This is used in enemy AI movement.

---

# Example 5: Early Exit Conditions

Some control structures stop code early.

```javascript
if (this.isKilling) return;
```

## Explanation

This prevents:
- unnecessary updates
- broken behavior
- wasted processing

Early exits make code more efficient.

---

# Why Control Structures Help My Game

Control structures improved my game by:
- controlling game logic flow
- managing enemy AI behavior
- handling collisions
- improving performance
- making decisions inside the game

Without them, the game would not respond dynamically to player actions.