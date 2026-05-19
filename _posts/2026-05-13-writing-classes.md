---
layout: post
title: Writing Classes in My Game
permalink: /writing-classes/
description: How classes are created and used in my JavaScript ocean game.
---

# Writing Classes in My Game

## What Are Classes?

A class is a blueprint used to create objects in programming.

Classes help organize code by grouping:
- properties
- variables
- methods
- behaviors

In my game, classes are used to create:
- the player
- enemies
- sharks
- NPCs
- scoring systems

This makes the game easier to manage and reuse.

---

# Example 1: Creating a Class

One class I created is called `GameScorer`.

```javascript
class GameScorer {
  constructor(gameEnv) {
    this.gameEnv = gameEnv;
    this.score = 0;
    this.coinsCollected = 0;
    this.totalCoins = 0;
  }
}
```

## Explanation

This class is responsible for:
- tracking score
- counting collected coins
- managing scoreboard information

The `constructor()` initializes values when the object is created.

---

# Example 2: Adding Methods to a Class

Classes can contain methods (functions).

```javascript
collectCoin(points = 10) {
  this.coinsCollected++;
  this.score += points;
  this.updateDisplay();
}
```

## Explanation

This method:
1. increases the coin count
2. adds points to the score
3. updates the scoreboard display

Methods allow objects to perform actions.

---

# Example 3: Creating Objects From Classes

After writing a class, objects can be created using `new`.

```javascript
gameEnv.gameScorer = new GameScorer(gameEnv);
```

## Explanation

This creates a new `GameScorer` object that the game can use during gameplay.

---

# Example 4: Player Class

My game engine also uses a `Player` class.

```javascript
{ class: Player, data: octopusData }
```

## Explanation

The `Player` class controls:
- movement
- animations
- collisions
- interactions

This allows the octopus character to behave like a playable object.

---

# Example 5: Shark Class

I also created a custom shark enemy class.

```javascript
import Shark from '@assets/js/GameEnginev1.1/Shark.js';
```

## Explanation

The shark class gives enemies custom behavior like:
- chasing the player
- movement logic
- collision behavior

Using separate classes keeps enemy systems organized.

---

# Why Writing Classes Is Important

Writing classes helped my project by:
- organizing large amounts of code
- making systems reusable
- reducing repeated code
- simplifying debugging
- improving readability

Without classes, the game would be much harder to expand and maintain.