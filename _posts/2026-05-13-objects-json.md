---
layout: post
title: Objects (JSON) in My Game
permalink: /objects-json/
description: How objects and JSON-style data are used in my JavaScript ocean game.
---

# Objects (JSON) in My Game

## What Are Objects?

Objects store related information using key-value pairs.

Example:

```javascript
const player = {
  name: "Octopus",
  health: 100
};
```

Objects are used to organize complex data in programming.

Games use objects for:
- players
- enemies
- settings
- positions
- animations
- configurations

My game heavily relies on objects to manage gameplay systems.

---

# What Is JSON?

JSON stands for:

```text
JavaScript Object Notation
```

JSON uses object-style formatting to organize data.

Example:

```javascript
{
  id: "EnemyElon",
  speed: 2.2
}
```

My game uses many JSON-style objects for configuration and game data.

---

# Why Objects Are Important

Without objects, game data would become disorganized.

Objects allow the game to group related information together, such as:
- positions
- animations
- image paths
- hitboxes
- movement settings

Objects make systems easier to manage and reuse.

---

# Example 1: Background Object

My game uses an object to configure the background.

```javascript
const bgData = {
  id: "Water",
  src: path + "/images/projects/ocean/bg/reef.png",
  pixels: { height: 597, width: 340 }
};
```

## Explanation

This object stores:
- background ID
- image path
- image size

All related data is grouped together.

---

# Example 2: Player Object

The octopus player uses a large object.

```javascript
const octopusData = {
  id: "Octopus",
  greeting: "Hi I am Octopus!",
  SCALE_FACTOR: 5
};
```

## Explanation

This object stores:
- player name
- dialogue
- animation settings
- movement information
- rendering configuration

Objects help organize complex character systems.

---

# Example 3: Position Objects

Objects are used for positions.

```javascript
INIT_POSITION: {
  x: width * 0.7,
  y: height * 0.6
}
```

## Explanation

This object stores:
- x position
- y position

Position objects help place game entities on the screen.

---

# Example 4: Hitbox Objects

Collision systems use objects.

```javascript
hitbox: {
  widthPercentage: 0.4,
  heightPercentage: 0.4
}
```

## Explanation

This object stores:
- collision width
- collision height

Objects keep collision settings organized.

---

# Example 5: Enemy Objects

Enemies are configured using reusable objects.

```javascript
const baseEnemy = {
  src: sprite_src_enemy,
  SCALE_FACTOR: 5,
  ANIMATION_RATE: 0
};
```

## Explanation

This object stores:
- enemy image data
- animation speed
- rendering settings
- movement configuration

Other enemies can reuse this object structure.

---

# Example 6: Goldfish Objects

Goldfish are created with object data.

```javascript
data: {
  id: `Goldfish${i}`,
  greeting: "+10 Points!"
}
```

## Explanation

Each goldfish object stores:
- unique IDs
- collectible behavior
- dialogue information

Objects allow every game entity to have its own properties.

---

# Example 7: Nested Objects

My game uses objects inside other objects.

```javascript
pixels: {
  width: 200,
  height: 100
}
```

## Explanation

This is called a nested object.

Nested objects help organize:
- dimensions
- positions
- animations
- grouped settings

This keeps code clean and readable.

---

# Why Objects (JSON) Help My Game

Objects improved my project by:
- organizing complex data
- grouping related properties together
- simplifying game configuration
- improving readability
- making systems reusable and scalable

Without objects, the game code would become difficult to manage.