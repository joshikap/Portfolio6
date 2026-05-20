---
layout: post
title: Nested Conditions in My Game
permalink: /nested-conditions/
description: How nested conditions are used in my JavaScript ocean game.
---

# Nested Conditions in My Game

## What Are Nested Conditions?

Nested conditions are conditionals placed inside other conditionals.

This means one condition is checked first, and then another condition is checked inside it.

Example structure:

```javascript
if (condition1) {

  if (condition2) {

  }

}
```

Nested conditions allow more advanced decision-making.

---

# Why Nested Conditions Are Important

Games often require multiple checks before an action happens.

For example:
- checking if a player collides with an enemy
- checking if damage cooldown is active
- checking if score should update

Nested conditions help organize these layered checks clearly.

---

# Example 1: Collision + Cooldown Check

My game uses nested conditions for collision detection.

```javascript
if (dist < 40) {

  if (!this.gameEnv.elonHitCooldown) {

    this.gameEnv.gameScorer.deductPoints(10);

  }

}
```

## Explanation

The first condition checks:
- if the player is close enough to the enemy

The nested condition checks:
- if cooldown is inactive

Only then does the game:
- deduct points
- apply collision effects

---

# Example 2: Preventing Repeated Damage

Nested conditions help stop repeated collisions.

```javascript
if (!this.gameEnv.elonHitCooldown) {

  this.gameEnv.elonHitCooldown = true;

  setTimeout(() => {
    this.gameEnv.elonHitCooldown = false;
  }, 1000);

}
```

## Explanation

This logic:
1. checks if cooldown is inactive
2. activates cooldown
3. waits 1 second
4. disables cooldown again

Nested logic helps control timing systems.

---

# Example 3: Enemy AI Decisions

Enemies use nested conditions to manage behavior.

```javascript
if (players.length === 0) return;

for (const player of players) {

  if (dist < minDist) {

    nearest = player;

  }

}
```

## Explanation

This checks:
- whether players exist
- whether a player is closer than the previous target

Nested conditions allow enemies to make smart decisions.

---

# Example 4: Score Protection Logic

Nested conditions protect game values.

```javascript
if (this.score < 0) {

  if (this.score !== 0) {

    this.score = 0;

  }

}
```

## Explanation

This ensures:
- negative scores are detected
- score resets safely
- unnecessary updates are avoided

---

# Example 5: Goldfish Collection Logic

Nested conditions are used during object interaction.

```javascript
if (fish) {

  if (gameEnv.gameScorer) {

    gameEnv.gameScorer.collectCoin(10);

  }

}
```

## Explanation

This checks:
- if the fish object exists
- if the scoring system exists
- then safely adds points

Nested conditions improve reliability and prevent errors.

---

# Why Nested Conditions Help My Game

Nested conditions improved my game by:
- allowing advanced decision-making
- organizing layered game logic
- improving collision systems
- controlling enemy AI behavior
- preventing invalid actions and errors

Without nested conditions, many game systems would be less reliable and harder to manage.