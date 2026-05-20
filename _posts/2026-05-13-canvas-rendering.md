---
layout: post
title: Canvas Rendering in My Game
permalink: /canvas-rendering/
description: How canvas rendering is used in my JavaScript ocean game.
---

# Canvas Rendering in My Game

## What Is Canvas Rendering?

Canvas rendering is the process of drawing graphics onto the screen.

Games use rendering systems to display:
- characters
- backgrounds
- enemies
- animations
- UI elements

My game uses canvas rendering to visually display the entire game world.

---

# Why Canvas Rendering Is Important

Without rendering, the player would not see:
- the octopus character
- enemies
- goldfish
- backgrounds
- score updates
- animations

Canvas rendering turns game data into visible gameplay.

---

# Example 1: Rendering the Background

My game renders an ocean background image.

```javascript
const bgData = {
  id: "Water",
  src: path + "/images/projects/ocean/bg/reef.png"
};
```

## Explanation

This rendering system:
- loads the reef image
- displays the ocean environment
- creates the game world background

The canvas continuously draws this image during gameplay.

---

# Example 2: Rendering the Player

The octopus player is rendered using sprite images.

```javascript
src: path + "/images/projects/ocean/player/octopus.png"
```

## Explanation

This image:
- represents the player visually
- appears on the screen
- animates during movement

The rendering system updates the sprite continuously.

---

# Example 3: Rendering Enemies

Enemy sprites are also rendered on the canvas.

```javascript
const sprite_src_enemy = path + "/images/projects/ocean/npc/elonMusk.png";
```

## Explanation

This rendering system:
- loads enemy images
- displays enemies visually
- updates enemy positions in real time

Enemies move smoothly because the canvas redraws every frame.

---

# Example 4: Rendering Goldfish

Goldfish collectibles are rendered as NPC objects.

```javascript
src: path + "/images/projects/ocean/npc/gold.png"
```

## Explanation

The game renders:
- collectible fish
- animated objects
- interactive items

Canvas rendering makes collectibles visible to the player.

---

# Example 5: Animation Rendering

The game renders animations using sprite sheets.

```javascript
orientation: { rows: 3, columns: 2 }
```

## Explanation

This controls:
- animation frames
- sprite directions
- movement animations

Rendering systems display different sprite frames over time.

---

# Example 6: Directional Rendering

The player changes appearance based on movement.

```javascript
left: { row: 1, start: 0, columns: 2 },
right: { row: 1, start: 0, columns: 2 },
up: { row: 2, start: 0, columns: 2 },
down: { row: 0, start: 0, columns: 2 },
```

## Explanation

The rendering system:
- changes animation direction
- updates sprite frames
- creates smooth movement visuals

This makes gameplay feel responsive.

---

# Example 7: Rendering Positions

Canvas rendering uses position values.

```javascript
INIT_POSITION: {
  x: width * 0.7,
  y: height * 0.6
}
```

## Explanation

The rendering engine uses:
- x coordinates
- y coordinates

to determine where objects appear on screen.

---

# Example 8: Rendering Scale

Objects are scaled visually.

```javascript
SCALE_FACTOR: 5
```

## Explanation

This controls:
- object size
- sprite scaling
- visual proportions

Different scale factors create different visual effects.

---

# Example 9: Rendering Updates

The game continuously redraws moving objects.

```javascript
update: function () {

}
```

## Explanation

The rendering loop:
- refreshes positions
- redraws sprites
- updates animations
- creates real-time gameplay

This allows movement and animation to appear smooth.

---

# Why Canvas Rendering Helps My Game

Canvas rendering improved my project by:
- displaying graphics visually
- creating animations
- rendering movement smoothly
- supporting enemy and player visuals
- making the game interactive and immersive

Without canvas rendering, the game would not have visible gameplay.