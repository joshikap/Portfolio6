---
layout: post
title: Data Types in My Game
permalink: /data-types/
description: How data types are used in my JavaScript ocean game.
---

# Data Types in My Game

## What Are Data Types?

Data types are different kinds of values used in programming.

They allow programs to store and work with information.

Common data types include:
- numbers
- strings
- booleans
- arrays
- objects

My game uses all of these to control gameplay systems.

---

# Why Data Types Are Important

Games need many kinds of information, such as:
- scores
- player names
- enemy positions
- collision states
- lists of objects

Different data types are used depending on what kind of data is needed.

---

# Example 1: Numbers

Numbers are used for calculations and positions.

```javascript
const speed = 2.2;
```

## Explanation

Numbers are used for:
- movement speed
- score values
- positions
- collision distances
- animation timing

Another example:

```javascript
this.score += points;
```

This updates the player's score numerically.

---

# Example 2: Strings

Strings store text.

```javascript
id: "EnemyElon"
```

## Explanation

Strings are used for:
- object IDs
- labels
- greetings
- names
- messages

Another example:

```javascript
greeting: "Hello! I'm a wizard! ✨"
```

This stores dialogue text for the NPC.

---

# Example 3: Booleans

Booleans store `true` or `false` values.

```javascript
this.gameEnv.elonHitCooldown = false;
```

## Explanation

Booleans are used for:
- collision cooldowns
- enemy states
- checking conditions
- controlling logic

Another example:

```javascript
if (!this.gameEnv.elonHitCooldown)
```

This checks whether cooldown is active.

---

# Example 4: Arrays

Arrays store lists of values or objects.

```javascript
const enemies = this.gameEnv.gameObjects.filter(
  obj => obj.spriteData?.id?.includes("EnemyElon")
);
```

## Explanation

Arrays are used to store:
- enemies
- players
- collectibles
- game objects

This allows the game to manage many objects at once.

---

# Example 5: Objects (JSON)

Objects store structured data using key-value pairs.

```javascript
const bgData = {
  id: "Water",
  src: path + "/images/projects/ocean/bg/reef.png"
};
```

## Explanation

Objects are used for:
- sprite configuration
- positions
- settings
- game data

Objects organize related information together.

---

# Example 6: Complex Game Object Data

My game uses large structured objects for characters.

```javascript
const octopusData = {
  id: "Octopus",
  SCALE_FACTOR: 5,
  ANIMATION_RATE: 100
};
```

## Explanation

This object stores:
- animation data
- rendering information
- movement settings
- character properties

Objects help organize complex systems.

---

# Why Data Types Help My Game

Data types improved my project by:
- organizing different kinds of information
- enabling calculations and logic
- storing game objects efficiently
- improving readability
- making systems easier to manage

Without data types, the game would not be able to properly store or process information.