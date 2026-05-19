---
layout: post
title: Constructor Chaining in My Game
permalink: /constructor-chaining/
description: How constructor chaining is used in my JavaScript ocean game.
---

# Constructor Chaining in My Game

## What Is Constructor Chaining?

Constructor chaining happens when a child class uses the constructor from a parent class.

This is usually done with:

```javascript
super()
```

The `super()` method allows the child class to inherit setup code from the parent class.

This helps:
- reuse initialization logic
- reduce repeated code
- simplify class setup

---

# Why Constructor Chaining Is Useful

Many game objects share similar setup behavior.

For example:
- position setup
- sprite configuration
- hitboxes
- animations
- game environment variables

Instead of rewriting the same constructor code, child classes can reuse parent constructors.

---

# Example 1: Shark Inheriting From NPC

My game uses inheritance with the shark enemy.

```javascript
class Shark extends Npc
```

## Explanation

The `Shark` class inherits from the `Npc` class.

This means the shark can reuse:
- NPC setup systems
- rendering systems
- positioning systems
- animation systems

The parent constructor helps initialize these features automatically.

---

# Example 2: Using super()

A constructor chain typically looks like this:

```javascript
constructor(data, gameEnv) {
  super(data, gameEnv);
}
```

## Explanation

The `super()` function:
1. calls the parent constructor
2. initializes inherited properties
3. allows the child class to add custom behavior afterward

This prevents duplicated setup code.

---

# Example 3: Reusing NPC Systems

The shark enemy can reuse NPC constructor logic.

```javascript
{ class: Shark, data: sprite_data_shark }
```

## Explanation

When the shark object is created:
- the parent NPC constructor runs first
- inherited properties are initialized
- the shark receives game object behavior automatically

Constructor chaining makes setup easier and more organized.

---

# Example 4: Shared Game Object Setup

Many objects in my game use shared setup systems.

```javascript
this.position.x += Math.cos(angle) * speed;
```

## Explanation

Objects inherit positioning and movement variables from parent systems.

This allows:
- reusable movement logic
- shared object properties
- consistent initialization

Constructor chaining helps organize these systems.

---

# Example 5: Reducing Duplicate Code

Without constructor chaining, every class would need separate setup code.

Instead of repeating:

```javascript
this.gameEnv = gameEnv;
this.position = data.position;
this.spriteData = data;
```

child classes can inherit setup automatically through `super()`.

## Explanation

This improves:
- readability
- maintainability
- scalability
- debugging

It also keeps the game engine cleaner.

---

# Why Constructor Chaining Helped My Game

Constructor chaining improved my project by:
- reducing repeated setup code
- simplifying class initialization
- improving organization
- making inheritance easier
- helping reusable game systems work together

Without constructor chaining, object setup would become repetitive and difficult to manage.