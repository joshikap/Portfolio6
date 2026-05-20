---
layout: post
title: Mathematical Operations in My Game
permalink: /mathematical/
description: How mathematical operations are used in my JavaScript ocean game.
---

# Mathematical Operations in My Game

## What Are Mathematical Operations?

Mathematical operations are calculations performed using numbers.

Common operations include:
- addition
- subtraction
- multiplication
- division
- distance calculations
- trigonometry

Games constantly use math for:
- movement
- scoring
- collision detection
- positioning
- animations

My game uses mathematical operations throughout its systems.

---

# Why Math Is Important in Games

Without mathematics, the game could not:
- move characters
- calculate collisions
- track score
- position enemies
- create smooth motion
- control AI movement

Math is one of the foundations of game development.

---

# Example 1: Adding Score

My game uses addition to increase score.

```javascript
this.score += points;
```

## Explanation

This mathematical operation:
- adds points to the score
- updates the scoreboard
- rewards the player

---

# Example 2: Subtracting Score

The game subtracts points after collisions.

```javascript
this.score -= points;
```

## Explanation

This operation:
- removes points
- applies penalties
- updates gameplay values

---

# Example 3: Multiplication for Positioning

The game uses multiplication to calculate positions.

```javascript
x: width * 0.7
```

## Explanation

This calculates:
- a percentage of screen width
- responsive object placement
- dynamic positioning

Another example:

```javascript
y: height * 0.6
```

This positions objects vertically.

---

# Example 4: Distance Formula

My game calculates distances between objects.

```javascript
const dist = Math.sqrt(dx * dx + dy * dy);
```

## Explanation

This uses:
- multiplication
- addition
- square roots

The calculation finds:
- the distance between player and enemy
- collision range
- nearest targets

This is essential for collision detection and AI.

---

# Example 5: Enemy Movement Math

Enemies move using trigonometry.

```javascript
this.position.x += Math.cos(angle) * speed;
this.position.y += Math.sin(angle) * speed;
```

## Explanation

This math:
- calculates movement direction
- moves enemies toward the player
- creates smooth chasing behavior

The game uses:
- cosine
- sine
- multiplication
- addition

---

# Example 6: Calculating Angles

The game calculates movement angles.

```javascript
const angle = Math.atan2(dy, dx);
```

## Explanation

This determines:
- the direction between two objects
- where enemies should move
- how AI tracks the player

This mathematical function is important for enemy movement systems.

---

# Example 7: Collision Range Check

Math is used for collision detection.

```javascript
if (dist < 40)
```

## Explanation

This compares:
- calculated distance
- collision range threshold

If objects are close enough:
- damage occurs
- score changes
- interactions activate

---

# Example 8: Animation Timing

Math controls animation speed.

```javascript
ANIMATION_RATE: 100
```

## Explanation

These numerical values affect:
- sprite animation timing
- movement smoothness
- gameplay pacing

---

# Example 9: Creating Multiple Objects

Math helps generate repeated objects.

```javascript
Array.from({ length: 10 })
```

## Explanation

This number:
- creates 10 goldfish
- controls object count
- scales gameplay systems

---

# Why Mathematical Operations Help My Game

Mathematical operations improved my project by:
- enabling movement systems
- controlling enemy AI
- calculating collisions
- managing score systems
- supporting animations and positioning

Without math, the game would not function properly.