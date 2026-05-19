---
layout: post
title: Iteration in My Game
permalink: /iteration/
description: How iteration (loops) is used in my JavaScript ocean game.
---

# Iteration in My Game

## What Is Iteration?

Iteration means repeating a block of code multiple times using loops.

In programming, iteration is used when you need to:
- go through lists
- repeat actions
- update multiple objects
- process game entities

Common loop types include:
- `for` loops
- `while` loops
- `forEach` loops

---

# Why Iteration Is Important in Games

Games constantly repeat actions every frame, such as:
- updating enemies
- checking collisions
- moving objects
- rendering animations

Without iteration, you would have to write separate code for every object, which is not scalable.

---

# Example 1: Looping Through Enemies

My game uses iteration to process all enemies.

```javascript
for (const enemy of enemies) {
  const dx = enemy.position.x - this.position.x;
  const dy = enemy.position.y - this.position.y;
}
```

## Explanation

This loop:
- goes through every enemy in the game
- calculates distance to the player
- helps determine movement behavior

---

# Example 2: Finding Goldfish Objects

Iteration is used to find specific objects.

```javascript
const fish = gameEnv.gameObjects.find(obj =>
  obj.spriteData?.id === `Goldfish${i}`
);
```

## Explanation

This searches through all game objects to:
- find a specific goldfish
- apply reactions (like collecting coins)
- remove it after collection

---

# Example 3: Looping Through Players

Enemies also use iteration to find players.

```javascript
const players = this.gameEnv.gameObjects.filter(
  obj => obj.constructor.name === "Player"
);
```

## Explanation

This loop:
- filters all game objects
- returns only player objects
- allows enemies to target the player

---

# Example 4: Calculating Nearest Target

Iteration helps enemies choose targets.

```javascript
for (const player of players) {
  const dx = player.position.x - this.position.x;
  const dy = player.position.y - this.position.y;
}
```

## Explanation

This repeats for every player:
- calculates distance
- compares values
- finds the closest player

---

# Example 5: Creating Multiple Objects

Iteration is used to generate multiple goldfish.

```javascript
Array.from({ length: 10 }).map((_, i) => ({
  class: Npc,
  data: { id: `Goldfish${i}` }
}));
```

## Explanation

This creates:
- 10 goldfish objects
- each with unique IDs
- without writing repeated code

---

# Why Iteration Helps My Game

Iteration improved my project by:
- handling multiple objects efficiently
- reducing repeated code
- improving performance
- enabling AI and collision systems
- making object management scalable

Without iteration, the game would not be able to handle multiple enemies or objects efficiently.
