---
layout: post
title: Inheritance in My Game
permalink: /inheritance-basic/
description: How inheritance is used in my JavaScript ocean game.
---

# Inheritance in My Game

## What Is Inheritance?

Inheritance is when one class gains features and behavior from another class.

This allows programmers to:
- reuse code
- reduce repetition
- organize systems more efficiently

A child class can inherit:
- properties
- methods
- behaviors

from a parent class.

---

# Why Inheritance Is Useful

Inheritance helps games because many objects share similar behavior.

For example:
- enemies move
- NPCs interact
- players update positions
- objects render on screen

Instead of rewriting the same code many times, inheritance allows classes to reuse existing systems.

---

# Example 1: Shark Inheriting From NPC

My game uses inheritance with the shark enemy.

```javascript
class Shark extends Npc
```

## Explanation

The `Shark` class inherits features from the `Npc` class.

This means the shark automatically receives:
- NPC behavior
- positioning systems
- rendering logic
- update systems
- game environment access

The shark can then add custom behavior on top of the inherited features.

---

# Example 2: Using Imported Classes

The shark class is imported into the game level.

```javascript
import Shark from '@assets/js/GameEnginev1.1/Shark.js';
```

## Explanation

This allows the game to create shark objects using the inherited class.

The shark behaves like an NPC but has custom enemy movement.

---

# Example 3: Creating the Shark Object

The inherited shark class is instantiated in the game.

```javascript
{ class: Shark, data: sprite_data_shark }
```

## Explanation

This creates a shark object using the inherited class.

The shark can:
- chase the player
- update movement
- interact with collisions
- use NPC systems automatically

Inheritance makes the shark system reusable and efficient.

---

# Example 4: Reusing Enemy Behavior

My game also reuses enemy systems through shared object structures.

```javascript
const baseEnemy = {
  src: sprite_src_enemy,
  SCALE_FACTOR: 5
};
```

## Explanation

This shared enemy structure acts similarly to inheritance.

Multiple enemies reuse:
- movement logic
- collision systems
- rendering settings

This prevents duplicated code.

---

# Example 5: Method Reuse

Inherited classes can reuse methods from parent classes.

```javascript
update: function () {

  const players = this.gameEnv.gameObjects.filter(
    obj => obj.constructor.name === "Player"
  );

}
```

## Explanation

The shark and NPC systems can both use update methods to:
- detect players
- move around the map
- react during gameplay

Inheritance allows child classes to share these behaviors.

---

# Why Inheritance Helped My Game

Inheritance improved my project by:
- reducing repeated code
- improving organization
- making enemy systems reusable
- simplifying updates
- making the game easier to expand

Without inheritance, every enemy would need completely separate code.