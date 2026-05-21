---
layout: post
codemirror: true
title: CSSE Objectives
description: A JavaScript game project demonstrating core Computer Science concepts including Object-Oriented Programming, inheritance, control structures, data types, and API integration.
permalink: /information-checklist/
---

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<style>

:root{
  --bg:#0a0a0a;
  --panel:#111;
  --panel2:#161616;
  --pink:#f52bc9;
  --pink-light:#ff5fd7;
  --purple:#7a5cff;
  --text:#d9d9d9;
}

body{
  font-family:'Inter', sans-serif;

  background:
    radial-gradient(circle at top left,
    rgba(245,43,201,0.15),
    transparent 30%),

    radial-gradient(circle at bottom right,
    rgba(122,92,255,0.12),
    transparent 30%),

    var(--bg);

  color:var(--text);
}

/* HERO */

.hero{
  text-align:center;
  padding:50px 20px 30px;
}

.hero h1{
  font-size:52px;
  font-weight:800;
  color:white;
  margin-bottom:12px;
}

/* PROGRESS */

.progress-wrapper{
  margin:25px 0 35px;
}

.progress-text{
  margin-bottom:10px;
  font-weight:600;
  color:white;
}

.progress-bar{
  width:100%;
  height:14px;
  background:#222;
  border-radius:999px;
  overflow:hidden;
}

.progress-fill{
  width:78%;
  height:100%;
  background:linear-gradient(
    90deg,
    var(--pink),
    var(--purple)
  );

  box-shadow:0 0 18px rgba(245,43,201,0.45);
}

/* TABLE */

.table-container{
  width:100%;
  overflow-x:auto;
  background:#0d0d0d;
  padding:25px;
  border-radius:18px;
}

table{
  width:100%;
  border-collapse:collapse;
  background:var(--panel);
  border:2px solid var(--pink);
  box-shadow:0 0 20px rgba(98,5,67,0.35);
}

th{
  background:#1a1a1a;
  color:var(--text);
  font-size:24px;
  text-align:left;
  padding:22px;
  border:1px solid var(--pink);
}

td{
  padding:22px;
  border:1px solid #f02bc5;
  vertical-align:top;
  font-size:18px;
  line-height:1.7;
  color:#cfcfcf;
}

tr{
  transition:
    transform 0.25s ease,
    box-shadow 0.25s ease,
    background 0.25s ease;
}

tr:nth-child(even){
  background:var(--panel2);
}

tr:hover{
  background:#1f1f1f;
  transform:translateY(-3px);
  box-shadow:0 0 18px rgba(245,43,201,0.2);
}

.objective{
  font-weight:700;
  color:white;
  width:25%;
}

.meaning{
  width:35%;
}

.applied{
  width:40%;
}

/* CODE */

.code{
  background:#2a2a2a;
  padding:4px 8px;
  border-radius:6px;
  color:white;
  font-family:Consolas, monospace;
}

/* BUTTON */

.learn-btn{
  display:inline-block;
  padding:12px 18px;
  background:var(--pink);
  color:white;
  text-decoration:none;
  border-radius:10px;
  font-weight:700;

  transition:
    transform 0.2s ease,
    background 0.2s ease,
    box-shadow 0.2s ease;

  margin-top:12px;
}

.learn-btn:hover{
  background:var(--pink-light);
  transform:scale(1.05);
  box-shadow:0 0 16px rgba(245,43,201,0.55);
}

/* DETAILS */

details{
  margin-top:18px;
  background:#1a1a1a;
  padding:14px;
  border-radius:10px;
  border:1px solid rgba(245,43,201,0.3);
}

summary{
  cursor:pointer;
  color:var(--pink-light);
  font-weight:700;
}

pre{
  margin-top:12px;
  background:#0f0f0f;
  padding:15px;
  border-radius:10px;
  overflow-x:auto;
  color:#dcdcdc;
}

/* ICONS */

.icon{
  margin-right:10px;
  color:var(--pink-light);
}

</style>

<div class="hero">
  <h1>🎮 CSSE Learning Objectives</h1>
</div>

<div class="progress-wrapper">

  <div class="progress-text">
    Project Completion Progress
  </div>

  <div class="progress-bar">
    <div class="progress-fill"></div>
  </div>

</div>

<div class="table-container">

<table>

<tr>
  <th>Learning Objective</th>
  <th>What It Means</th>
  <th>How It’s Applied</th>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-gamepad icon"></i>
Object-Oriented Programming
</td>

<td class="meaning">
Organizing code using classes and objects.
</td>

<td class="applied">

Used to create game characters,
enemies, and reusable systems.

<br><br>

<a href="/oop-explanation/" class="learn-btn">
View Example
</a>

<details>
<summary>Preview Code</summary>

<pre>
class Player {

  constructor(name){
    this.name = name;
  }

  move(){
    console.log("Moving");
  }

}
</pre>

</details>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-cubes icon"></i>
Writing Classes
</td>

<td class="meaning">
Creating blueprints for objects
with properties and methods.
</td>

<td class="applied">

Create classes like
<span class="code">Player</span>
and
<span class="code">Enemy</span>.

<br><br>

<a href="/writing-classes/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-code icon"></i>
Methods & Parameters
</td>

<td class="meaning">
Functions inside classes that can
accept data.
</td>

<td class="applied">

Example:
<span class="code">
move(direction, speed)
</span>

<br><br>

<a href="/methods-parameters/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-cube icon"></i>
Instantiation & Objects
</td>

<td class="meaning">
Creating usable objects from classes.
</td>

<td class="applied">

Example:
<span class="code">
const player = new Player()
</span>

<br><br>

<a href="/instantiation-objects/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-diagram-project icon"></i>
Inheritance (Basic)
</td>

<td class="meaning">
One class can inherit features from another class.
</td>

<td class="applied">

Example:
<span class="code">
class Enemy extends Character
</span>

<br><br>

<a href="/inheritance-basic/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-rotate icon"></i>
Method Overriding
</td>

<td class="meaning">
Replacing a parent class method with a custom version.
</td>

<td class="applied">

Override
<span class="code">update()</span>
or
<span class="code">draw()</span>

<br><br>

<a href="/method-overriding/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-link icon"></i>
Constructor Chaining
</td>

<td class="meaning">
Using parent constructors inside child classes.
</td>

<td class="applied">

Example:
<span class="code">super(data)</span>

<br><br>

<a href="/constructor-chaining/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-code-branch icon"></i>
Control Structures
</td>

<td class="meaning">
Logic that controls program flow.
</td>

<td class="applied">

Used with loops and conditional statements.

<br><br>

<a href="/control-structures/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-repeat icon"></i>
Iteration
</td>

<td class="meaning">
Repeating code using loops.
</td>

<td class="applied">

Example:
<span class="code">for</span>
and
<span class="code">while</span>
loops.

<br><br>

<a href="/iteration/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-code-compare icon"></i>
Conditionals
</td>

<td class="meaning">
Running code only if conditions are true.
</td>

<td class="applied">

Example:
<span class="code">
if (health <= 0)
</span>

<br><br>

<a href="/conditionals/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-layer-group icon"></i>
Nested Conditions
</td>

<td class="meaning">
Conditions placed inside other conditions.
</td>

<td class="applied">

Used for advanced game logic checks.

<br><br>

<a href="/nested-conditions/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-database icon"></i>
Data Types
</td>

<td class="meaning">
Different kinds of data used in programming.
</td>

<td class="applied">

Includes numbers, strings, booleans,
arrays, and objects.

<br><br>

<a href="/data-types/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-hashtag icon"></i>
Numbers
</td>

<td class="meaning">
Numeric values used in calculations.
</td>

<td class="applied">

Used for score, speed,
damage, and positions.

<br><br>

<a href="/numbers/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-font icon"></i>
Strings
</td>

<td class="meaning">
Text values stored in code.
</td>

<td class="applied">

Used for names,
dialogue, and labels.

<br><br>

<a href="/strings/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-toggle-on icon"></i>
Booleans
</td>

<td class="meaning">
True or false values.
</td>

<td class="applied">

Example:
<span class="code">
isAlive = true
</span>

<br><br>

<a href="/booleans/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-list icon"></i>
Arrays
</td>

<td class="meaning">
Lists that store multiple values.
</td>

<td class="applied">

Used to store enemies,
bullets, or items.

<br><br>

<a href="/arrays/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-brackets-curly icon"></i>
Objects (JSON)
</td>

<td class="meaning">
Structured data using key-value pairs.
</td>

<td class="applied">

Used for game configuration and settings.

<br><br>

<a href="/objects-json/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-calculator icon"></i>
Operators
</td>

<td class="meaning">
Symbols used for calculations and comparisons.
</td>

<td class="applied">

Examples:
<span class="code">+</span>,
<span class="code">-</span>,
<span class="code">===</span>

<br><br>

<a href="/operators/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-square-root-variable icon"></i>
Mathematical
</td>

<td class="meaning">
Performing arithmetic calculations.
</td>

<td class="applied">

Used for movement,
collision, and scoring systems.

<br><br>

<a href="/mathematical/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-quote-left icon"></i>
String Operations
</td>

<td class="meaning">
Manipulating and combining text.
</td>

<td class="applied">

Example:
<span class="code">
"Score: " + points
</span>

<br><br>

<a href="/string-operations/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-circle-check icon"></i>
Boolean Expressions
</td>

<td class="meaning">
Expressions that evaluate to true or false.
</td>

<td class="applied">

Used in game decision-making logic.

<br><br>

<a href="/boolean-expressions/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-right-left icon"></i>
Input/Output
</td>

<td class="meaning">
Receiving user input and displaying results.
</td>

<td class="applied">

Used for controls,
menus, and game feedback.

<br><br>

<a href="/input-output/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-keyboard icon"></i>
Keyboard Input
</td>

<td class="meaning">
Detecting keyboard interactions.
</td>

<td class="applied">

Used for player movement and controls.

<br><br>

<a href="/keyboard-input/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-display icon"></i>
Canvas Rendering
</td>

<td class="meaning">
Drawing graphics onto the screen.
</td>

<td class="applied">

Used to render game characters and backgrounds.

<br><br>

<a href="/canvas-rendering/" class="learn-btn">
View Example
</a>

</td>
</tr>

<tr>
<td class="objective">
<i class="fa-solid fa-sliders icon"></i>
GameEnv Configuration
</td>

<td class="meaning">
Setting up the game environment and settings.
</td>

<td class="applied">

Used to configure levels,
objects, and gameplay values.

<br><br>

<a href="/gameenv-configuration/" class="learn-btn">
View Example
</a>

</td>
</tr>

</table>

</div>

<!-- CHALLENGES SECTION -->
<div style="margin:60px 20px; padding:30px; background:#0d0d0d; border-radius:18px; border:1px solid rgba(245,43,201,0.3);">

  <h2 style="color:white; font-size:34px; margin-bottom:20px;">
    Problems We Faced While Making the Game
  </h2>

  <p style="color:#cfcfcf; font-size:18px; margin-bottom:20px;">
    While building our game, we ran into a few problems. Here are the main ones and what we learned:
  </p>

  <div style="color:#cfcfcf; font-size:18px; line-height:1.9;">

    <p>• We got confused with <b>classes and objects</b> at first because there were a lot of files like <code class="code">Player</code>, <code class="code">Npc</code>, and enemies.</p>

    <p>• <b>Inheritance</b> was hard because we tried to make enemies act differently, but sometimes they still used the same code and acted wrong.</p>

    <p>• We had problems with <b>method overriding</b> because changing the <code class="code">update()</code> function sometimes broke movement or made things stop working.</p>

    <p>• <b>Collision detection</b> was an issue because the player was losing points too fast, so we added a cooldown (<code class="code">elonHitCooldown</code>) to fix it.</p>

    <p>• <b>If statements and logic</b> were tricky because sometimes enemies would not follow the player correctly or would target the wrong thing.</p>

    <p>• When using <b>arrays and loops</b>, we had issues where removed objects (like collected fish) were still causing bugs.</p>

    <p>• Our <b>score system</b> didn’t always update correctly until we put it into a separate class called <code class="code">GameScorer</code>.</p>

    <p>• We also had small bugs with <b>math and positioning</b> like distance calculations, which caused enemies to move weirdly.</p>

  </div>

  <p style="margin-top:25px; color:#cfcfcf; font-size:18px; line-height:1.8;">
    Overall, these problems helped us understand how all the CSSE concepts connect when making a real game.
  </p>

</div>