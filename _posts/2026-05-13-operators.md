---
layout: post
title: Operators in My Game
permalink: /operators/
description: How operators are used in my JavaScript ocean game.
---

# Operators in My Game

## What Are Operators?

Operators are symbols used to perform actions in programming.

Operators can:
- perform math
- compare values
- assign values
- combine data
- control logic

Games constantly use operators to manage gameplay systems.

---

# Types of Operators Used in My Game

My game uses several types of operators, including:
- arithmetic operators
- assignment operators
- comparison operators
- logical operators
- increment operators

---

# Example 1: Addition Operator

My game uses the `+` operator to increase score.

```javascript
this.score += points;
```

## Explanation

This operator:
- adds points to the score
- updates gameplay values
- changes the scoreboard

The `+=` operator is a shortcut for:

```javascript
this.score = this.score + points;
```

---

# Example 2: Subtraction Operator

The game removes points after collisions.

```javascript
this.score -= points;
```

## Explanation

This operator:
- subtracts points
- applies penalties
- updates the player's score

The `-=` operator combines subtraction and assignment.

---

# Example 3: Comparison Operators

The game compares values using operators.

```javascript
if (dist < 40)
```

## Explanation

The `<` operator checks:
- whether distance is less than 40
- if objects are close enough to collide

This returns either:
- `true`
- `false`

---

# Example 4: Equality Operators

My game checks exact values.

```javascript
obj.constructor.name === "Player"
```

## Explanation

The `===` operator checks:
- whether values are exactly equal
- both value and type

This helps identify player objects safely.

---

# Example 5: Assignment Operators

The game stores values using assignment.

```javascript
this.gameEnv.elonHitCooldown = true;
```

## Explanation

The `=` operator:
- assigns values
- updates variables
- changes game states

Assignment operators are used constantly in programming.

---

# Example 6: Multiplication Operators

The game uses multiplication for positioning.

```javascript
x: width * 0.7
```

## Explanation

The `*` operator:
- multiplies values
- calculates positions
- scales objects dynamically

This helps make the game responsive to screen size.

---

# Example 7: Logical Operators

Logical operators combine conditions.

```javascript
if (!this.gameEnv.elonHitCooldown)
```

## Explanation

The `!` operator means:
- NOT

This checks whether cooldown is false.

Logical operators help control game logic.

---

# Example 8: Incrementing Arrays

Operators are used in loops and iteration.

```javascript
Array.from({ length: 10 })
```

## Explanation

This uses numbers and object operators together to:
- create multiple objects
- generate arrays
- build scalable systems

---

# Example 9: Mathematical Movement Calculations

Operators help move enemies.

```javascript
this.position.x += Math.cos(angle) * speed;
```

## Explanation

This line uses:
- addition
- multiplication
- assignment

Together, these operators:
- calculate movement
- update positions
- create smooth enemy motion

---

# Why Operators Help My Game

Operators improved my project by:
- enabling calculations
- controlling game logic
- updating scores
- handling collisions
- supporting movement systems

Without operators, the game could not perform calculations or make decisions.