---
layout: post
title: Methods & Parameters in My Game
permalink: /methods-parameters/
description: How methods and parameters are used in my JavaScript ocean game.
---

# Methods & Parameters in My Game

## What Are Methods?

Methods are functions that belong to classes or objects.

Methods allow objects in a game to:
- move
- update
- interact
- perform actions

In my game, methods are used for:
- collecting coins
- enemy movement
- scoreboard updates
- collision systems
- rendering behavior

---

# What Are Parameters?

Parameters are pieces of data passed into methods.

They allow methods to work with different values.

Example:

```javascript
move(direction, speed)
```

Here:
- `direction` is a parameter
- `speed` is a parameter

Parameters make code flexible and reusable.

---

# Example 1: collectCoin Method

One method in my game is `collectCoin()`.

```javascript
collectCoin(points = 10) {
  this.coinsCollected++;
  this.score += points;
  this.updateDisplay();
}
```

## Explanation

This method:
1. increases collected coins
2. adds points to the score
3. updates the scoreboard

The parameter:

```javascript
points = 10
```

allows different coin values to be added.

---

# Example 2: deductPoints Method

Another method in my game removes points.

```javascript
deductPoints(points = 10) {
  this.score -= points;

  if (this.score < 0) {
    this.score = 0;
  }

  this.updateDisplay();
}
```

## Explanation

This method:
- subtracts points
- prevents negative scores
- updates the scoreboard

The parameter `points` controls how many points are removed.

---

# Example 3: Enemy Update Method

Enemies use an `update()` method.

```javascript
update: function () {

  const players = this.gameEnv.gameObjects.filter(
    obj => obj.constructor.name === "Player"
  );

}
```

## Explanation

The `update()` method runs repeatedly during gameplay.

It allows enemies to:
- detect players
- move toward the player
- react during the game

Methods make enemy behavior dynamic.

---

# Example 4: Collision Detection

The player also uses methods for collisions.

```javascript
if (dist < 40) {

  if (!this.gameEnv.elonHitCooldown) {

    this.gameEnv.gameScorer.deductPoints(10);

  }
}
```

## Explanation

This logic checks:
- distance between objects
- whether damage cooldown is active
- when to deduct points

Methods help organize collision systems cleanly.

---

# Why Methods & Parameters Are Important

Methods and parameters helped my project by:
- organizing game logic
- making code reusable
- reducing repeated code
- allowing flexible behaviors
- simplifying updates and debugging

Without methods and parameters, the game systems would be much harder to manage.