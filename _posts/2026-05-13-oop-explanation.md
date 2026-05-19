---
layout: post
title: Object-Oriented Programming in My Game
permalink: /oop-explanation
description: How Object-Oriented Programming is used in my JavaScript ocean game.
---

# Object-Oriented Programming in My Game

## What is Object-Oriented Programming?

Object-Oriented Programming (OOP) is a programming style that organizes code into classes and objects.

A class acts like a blueprint, while objects are created from that blueprint.

My game uses OOP to organize:
- the player
- enemies
- NPCs
- scoring systems
- game environments

This makes the code easier to reuse, update, and expand.

---

# Example 1: Creating a Class

In my game, I created a class called `GameScorer`.

```javascript
class GameScorer {
  constructor(gameEnv) {
    this.gameEnv = gameEnv;
    this.score = 0;
    this.coinsCollected = 0;
  }
}

---

# Example 2: Creating Objects (Instantiation)

Objects are created using the new keyword.

gameEnv.gameScorer = new GameScorer(gameEnv);

This creates a new GameScorer object that the game can use during gameplay.

---

# Example 4: Reusable Enemy System

I used object-oriented design to create reusable enemy objects.

const baseEnemy = {
  src: sprite_src_enemy,
  SCALE_FACTOR: 5,

  update: function () {
    const players = this.gameEnv.gameObjects.filter(
      obj => obj.constructor.name === "Player"
    );
  }
};

Explanation

This enemy system:

searches for players
follows the nearest player
updates enemy movement automatically

The same enemy logic can be reused for multiple enemies.

---