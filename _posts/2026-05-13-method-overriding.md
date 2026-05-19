---
layout: post
title: Method Overriding in My Game
permalink: /method-overriding/
description: How method overriding is used in my JavaScript ocean game.
---

# Method Overriding in My Game

## What Is Method Overriding?

Method overriding happens when a child class replaces a method from a parent class with its own custom version.

This allows objects to:
- behave differently
- customize functionality
- reuse parent systems while changing behavior

Overriding is commonly used in games for:
- enemy AI
- movement systems
- rendering
- collisions
- animations

---

# Why Method Overriding Is Useful

Many game objects share similar systems, but they should not all behave exactly the same.

For example:
- sharks move differently from NPCs
- enemies behave differently from players
- objects can have unique update behavior

Method overriding allows classes to customize these behaviors.

---

# Example 1: Custom Update Method

My game uses custom `update()` methods.

```javascript
update: function () {

  if (this.isKilling) return;

  const players = this.gameEnv.gameObjects.filter(
    obj => obj.constructor.name === "Player"
  );

}
```

## Explanation

This overridden `update()` method allows enemies to:
- detect players
- run AI logic
- update movement every frame

The custom version replaces default behavior with enemy-specific behavior.

---

# Example 2: Shark Movement Override

The shark enemy has its own movement system.

```javascript
const speed = 2.2;

this.position.x += Math.cos(angle) * speed;
this.position.y += Math.sin(angle) * speed;
```

## Explanation

This overridden behavior makes the shark:
- move faster
- chase the player
- behave differently from normal NPCs

Method overriding allows specialized enemy behavior.

---

# Example 3: Player Collision Override

The player object also overrides update behavior.

```javascript
update: function () {

  const enemies = this.gameEnv.gameObjects.filter(
    obj => obj.spriteData?.id?.includes("EnemyElon")
  );

}
```

## Explanation

This custom update method checks:
- nearby enemies
- collision distances
- score deduction logic

The player object uses its own custom behavior during gameplay.

---

# Example 4: Collision Reaction Override

The goldfish NPC overrides interaction behavior using a custom reaction method.

```javascript
reaction: function () {

  gameEnv.gameScorer.collectCoin(10);

}
```

## Explanation

This overridden method:
- increases score
- destroys the fish object
- updates the scoreboard

Different NPCs can react differently using overridden methods.

---

# Example 5: Reusable Systems With Custom Behavior

Enemies reuse the same base structure but override movement logic.

```javascript
const baseEnemy = {

  update: function () {

    const speed = 1.2;

  }

};
```

## Explanation

Each enemy can:
- reuse common systems
- customize speed
- customize movement
- customize interactions

Method overriding makes enemies flexible and reusable.

---

# Why Method Overriding Helped My Game

Method overriding improved my project by:
- allowing custom enemy behavior
- reducing repeated code
- improving game organization
- making systems reusable
- simplifying AI and collision systems

Without method overriding, every object would require completely separate code.