---
layout: post
title: Boolean Expressions in My Game
permalink: /boolean-expressions/
description: How boolean expressions are used in my JavaScript ocean game.
---

# Boolean Expressions in My Game

## What Are Boolean Expressions?

Boolean expressions are statements that evaluate to either:

```javascript
true
```

or

```javascript
false
```

They are used to make decisions in programming.

Games use boolean expressions for:
- collision detection
- enemy behavior
- score conditions
- game states
- input handling

My game uses boolean expressions constantly in gameplay logic.

---

# Why Boolean Expressions Are Important

Without boolean expressions, the game could not:
- make decisions
- detect collisions
- control AI behavior
- manage conditions
- respond to player actions

Boolean expressions are the foundation of game logic.

---

# Example 1: Collision Check

My game uses boolean expressions to detect collisions.

```javascript
if (dist < 40)
```

## Explanation

This expression evaluates to:
- `true` if objects are close enough
- `false` if they are too far apart

It controls when:
- damage happens
- score changes
- interactions trigger

---

# Example 2: Equality Check

The game checks exact matches using boolean expressions.

```javascript
obj.constructor.name === "Player"
```

## Explanation

This evaluates to:
- `true` if the object is a Player
- `false` otherwise

It is used for:
- filtering objects
- enemy targeting
- game logic decisions

---

# Example 3: String Boolean Expression

My game checks if text contains certain values.

```javascript
obj.spriteData?.id?.includes("EnemyElon")
```

## Explanation

This returns:
- `true` if the string contains "EnemyElon"
- `false` if it does not

Used for:
- enemy detection
- filtering arrays
- gameplay logic

---

# Example 4: Boolean Expressions in Conditions

Boolean expressions are used inside if statements.

```javascript
if (!this.gameEnv.elonHitCooldown)
```

## Explanation

This expression:
- evaluates cooldown state
- returns true or false
- controls whether damage is applied

The `!` operator reverses the boolean value.

---

# Example 5: Range Comparison

My game uses comparison expressions for AI movement.

```javascript
if (dist < minDist)
```

## Explanation

This evaluates:
- whether a player is closer than previous target
- updates nearest enemy target

It helps control enemy AI behavior.

---

# Example 6: Object Existence Check

Boolean expressions prevent errors.

```javascript
if (fish)
```

## Explanation

This evaluates:
- true if the object exists
- false if it is undefined or null

It ensures safe interactions in the game.

---

# Example 7: Score Validation

The game uses boolean expressions for score rules.

```javascript
if (this.score < 0)
```

## Explanation

This evaluates:
- true if score is negative
- false otherwise

Used to prevent invalid score values.

---

# Example 8: Combined Boolean Logic

My game uses multiple boolean expressions together.

```javascript
if (dist < 40 && !this.gameEnv.elonHitCooldown)
```

## Explanation

This evaluates to true only if:
- player is close enough
- cooldown is not active

This controls damage logic efficiently.

---

# Why Boolean Expressions Help My Game

Boolean expressions improved my project by:
- enabling decision-making
- controlling collisions and interactions
- managing enemy AI behavior
- preventing errors
- supporting gameplay logic

Without boolean expressions, the game would not be interactive or functional.