---
layout: post
title: Input/Output in My Game
permalink: /input-output/
description: How input and output systems are used in my JavaScript ocean game.
---

# Input/Output in My Game

## What Is Input/Output?

Input/Output (I/O) refers to:
- receiving information from the user (input)
- displaying information back to the user (output)

Games constantly use input and output systems.

Examples include:
- keyboard controls
- mouse input
- score displays
- graphics rendering
- dialogue systems

My game uses both input and output throughout gameplay.

---

# Why Input/Output Is Important

Without input and output, the game could not:
- receive player controls
- display graphics
- show score updates
- communicate information
- create interaction

Input and output make the game interactive.

---

# Example 1: Keyboard Input

My game receives player movement input from the keyboard.

```javascript
obj.constructor.name === "Player"
```

## Explanation

The Player system responds to:
- keyboard controls
- movement commands
- gameplay actions

Player input allows the user to control the octopus character.

---

# Example 2: Scoreboard Output

The game displays score information to the screen.

```javascript
this.scoreboard.innerHTML = `
  💰 Collected: ${this.coinsCollected}/${this.totalCoins}<br>
  ⭐ Score: ${this.score}
`;
```

## Explanation

This output system:
- updates the scoreboard
- displays collected coins
- shows current score

The player receives live feedback during gameplay.

---

# Example 3: Creating HTML Output

The game dynamically creates output elements.

```javascript
this.scoreboard = document.createElement('div');
```

## Explanation

This creates:
- a scoreboard element
- visual UI output
- an on-screen display

The game uses HTML output to communicate information.

---

# Example 4: Styling Visual Output

The scoreboard uses visual output styling.

```javascript
this.scoreboard.style.cssText = `
  position: fixed;
  top: 20px;
`;
```

## Explanation

This controls:
- scoreboard position
- colors
- font styles
- appearance on screen

Output systems improve the player experience.

---

# Example 5: Canvas & Sprite Rendering

The game outputs graphics using sprites.

```javascript
src: path + "/images/projects/ocean/player/octopus.png"
```

## Explanation

This output system:
- displays images
- renders characters
- creates visual gameplay

The player sees all game graphics through rendering output.

---

# Example 6: NPC Dialogue Output

The game displays text dialogue.

```javascript
greeting: "Hello! I'm a wizard! ✨"
```

## Explanation

This output:
- communicates with the player
- displays NPC text
- improves interaction

Dialogue is another form of game output.

---

# Example 7: Collision Feedback

The game outputs gameplay changes after collisions.

```javascript
this.gameEnv.gameScorer.deductPoints(10);
```

## Explanation

This updates:
- score values
- scoreboard output
- gameplay feedback

The player immediately sees the result of collisions.

---

# Example 8: Coin Collection Output

Collecting goldfish updates the UI.

```javascript
this.gameEnv.gameScorer.collectCoin(10);
```

## Explanation

This outputs:
- updated score
- collected coin count
- reward feedback

This helps the player track progress.

---

# Why Input/Output Helps My Game

Input/output systems improved my project by:
- enabling player interaction
- displaying gameplay information
- updating score systems
- rendering graphics and dialogue
- making the game responsive and interactive

Without input/output systems, the game would not function as an interactive experience.