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
   radial-gradient(circle at top left, rgba(245,43,201,0.15), transparent 30%),
   radial-gradient(circle at bottom right, rgba(122,92,255,0.12), transparent 30%),
   var(--bg);
 color:var(--text);
}


.hero{
 text-align:center;
 padding:50px 20px 30px;
}


.hero h1{
 font-size:52px;
 font-weight:800;
 color:white;
}


.progress-wrapper{ margin:25px 0 35px; }
.progress-text{ margin-bottom:10px; font-weight:600; color:white; }


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
 background:linear-gradient(90deg,var(--pink),var(--purple));
 box-shadow:0 0 18px rgba(245,43,201,0.45);
}


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
}


th{
 background:#1a1a1a;
 padding:22px;
 font-size:24px;
 border:1px solid var(--pink);
}


td{
 padding:22px;
 border:1px solid #f02bc5;
 font-size:18px;
 vertical-align:top;
}


tr:nth-child(even){ background:var(--panel2); }

tr{
  transition: 0.25s ease;
}

tr:hover{
  box-shadow:
    0 0 0 1px rgba(245, 43, 201, 0.6),
    0 0 20px rgba(245, 43, 201, 0.25),
    0 0 40px rgba(122, 92, 255, 0.15);
  transform: translateY(-2px);
  position: relative;
  z-index: 2;
}

.learn-btn{
 display:inline-block;
 padding:12px 18px;
 background:var(--pink);
 color:white;
 text-decoration:none;
 border-radius:10px;
 font-weight:700;
 margin-top:10px;
 margin-right:10px;
}

.learn-btn:hover{
 background:var(--pink-light);
}

details{
 margin-top:12px;
 background:#1a1a1a;
 padding:12px;
 border-radius:10px;
 border:1px solid rgba(245,43,201,0.3);
}

summary{
 cursor:pointer;
 color:var(--pink-light);
 font-weight:700;
}

pre{
 margin-top:10px;
 background:#0f0f0f;
 padding:12px;
 border-radius:10px;
 overflow-x:auto;
}

.code{
 background:#2a2a2a;
 padding:4px 8px;
 border-radius:6px;
}
</style>


<div class="hero">
 <h1>🎮 CSSE Learning Objectives</h1>
</div>


<div class="progress-wrapper">
 <div class="progress-text">Project Completion Progress</div>
 <div class="progress-bar"><div class="progress-fill"></div></div>
</div>


<div class="table-container">
<table>

<tr>
<th>Learning Objective</th>
<th>What It Means</th>
<th>How It’s Applied</th>
</tr>

<tr>
  <td>Object-Oriented Programming</td>
  <td>Organizing code using classes and objects.</td>
  <td>
    Used for game characters and systems.
    <br>

    <a class="learn-btn" href="/oop-explanation/">
      View Example
    </a>

    <a class="learn-btn" href="#">
      Preview Code
    </a>

    <details>
      <summary>Show Code</summary>

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
<td>Writing Classes</td>
<td>Creating reusable blueprints that define properties and behaviors for objects in the game.</td>
<td>
Player and Enemy classes.
<br>
<a class="learn-btn" href="/writing-classes/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
class Enemy {
 constructor(type){
   this.type = type;
 }
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Methods & Parameters</td>
<td>Functions inside classes that allow objects to perform actions and accept inputs to change behavior dynamically.</td>
<td>
move(direction, speed)
<br>
<a class="learn-btn" href="/methods-parameters/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
move(direction, speed){
 this.x += speed;
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Instantiation & Objects</td>
<td>Creating real usable instances from classes so the game can generate active characters and elements.</td>
<td>
const player = new Player()
<br>
<a class="learn-btn" href="/instantiation-objects/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
const player = new Player("Alex");
</pre>
</details>
</td>
</tr>

<tr>
<td>Inheritance (Basic)</td>
<td>Allowing one class to inherit properties and methods from another class to reduce repeated code and build structured hierarchies.</td>
<td>
Enemy extends Character
<br>
<a class="learn-btn" href="/inheritance-basic/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
class Enemy extends Character {}
</pre>
</details>
</td>
</tr>

<tr>
<td>Method Overriding</td>
<td>Redefining a method in a child class to change or customize behavior inherited from a parent class.</td>
<td>
override update()
<br>
<a class="learn-btn" href="/method-overriding/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
update(){
 console.log("custom update");
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Constructor Chaining</td>
<td>Using super() to call the parent class constructor so shared properties are properly initialized in child classes.</td>
<td>
super(data)
<br>
<a class="learn-btn" href="/constructor-chaining/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
constructor(){
 super();
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Control Structures</td>
<td>Statements that control the flow of the program by making decisions or repeating actions based on conditions.</td>
<td>
if / loops
<br>
<a class="learn-btn" href="/control-structures/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
if (score > 10){
 win();
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Iteration</td>
<td>Repeating a block of code multiple times using loops to handle repeated actions efficiently.</td>
<td>
for / while
<br>
<a class="learn-btn" href="/iteration/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
for(let i=0;i<10;i++){
 console.log(i);
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Conditionals</td>
<td>Decision-making statements that execute different code depending on whether a condition is true or false.</td>
<td>
if (health <= 0)
<br>
<a class="learn-btn" href="/conditionals/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
if (health <= 0){
 gameOver();
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Nested Conditions</td>
<td>Using multiple conditional statements inside one another to handle more complex decision-making logic.</td>
<td>
Advanced game logic
<br>
<a class="learn-btn" href="/nested-conditions/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
if (x > 10){
 if (y > 5){
   console.log("hit");
 }
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Data Types</td>
<td>Different kinds of values used in programming such as numbers, text, and true/false values that define how data behaves.</td>
<td>
numbers, strings, booleans
<br>
<a class="learn-btn" href="/data-types/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
let score = 10;
let name = "Player";
let alive = true;
</pre>
</details>
</td>
</tr>

<tr>
<td>Numbers</td>
<td>Numeric data used for calculations such as scoring, movement speed, health, and other measurable values in the game.</td>
<td>
score, speed, damage
<br>
<a class="learn-btn" href="/numbers/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
let score = 100;
</pre>
</details>
</td>
</tr>

<tr>
<td>Strings</td>
<td>Text-based data used for names, dialogue, labels, and any readable content displayed to the user.</td>
<td>
names, dialogue
<br>
<a class="learn-btn" href="/strings/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
let name = "Hero";
</pre>
</details>
</td>
</tr>

<tr>
<td>Booleans</td>
<td>Values that represent true or false states, commonly used for game states like alive/dead or active/inactive.</td>
<td>
isAlive = true
<br>
<a class="learn-btn" href="/booleans/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
let isAlive = true;
</pre>
</details>
</td>
</tr>

<tr>
<td>Arrays</td>
<td>Ordered lists that store multiple values in a single variable, used for managing groups like enemies or items.</td>
<td>
enemies, items
<br>
<a class="learn-btn" href="/arrays/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
let enemies = [];
</pre>
</details>
</td>
</tr>

<tr>
<td>Objects (JSON)</td>
<td>Structured data made of key-value pairs used to represent complex entities like players, settings, or game states.</td>
<td>
game settings
<br>
<a class="learn-btn" href="/objects-json/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
let player = { name:"Alex", hp:100 };
</pre>
</details>
</td>
</tr>

<tr>
<td>Operators</td>
<td>Symbols used to perform calculations or comparisons, such as addition, subtraction, and equality checks.</td>
<td>
calculations & comparisons
<br>
<a class="learn-btn" href="/operators/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
let total = a + b;
</pre>
</details>
</td>
</tr>

<tr>
<td>Mathematical</td>
<td>Math operations used to calculate movement, distance, physics, and scoring mechanics in the game.</td>
<td>
movement, scoring
<br>
<a class="learn-btn" href="/mathematical/">View Example</a>
<a class="learn-btn">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
distance = Math.sqrt(x*x + y*y);
</pre>
</details>
</td>
</tr>

<tr>
<td>String Operations</td>
<td>Combining and manipulating text values to create messages, scores, and dynamic UI text.</td>
<td>
"Score: " + points
<br>
<a class="learn-btn" href="/string-operations/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
let msg = "Score: " + score;
</pre>
</details>
</td>
</tr>

<tr>
<td>Boolean Expressions</td>
<td>Logical conditions that combine multiple comparisons to make complex decisions in gameplay.</td>
<td>
decision making
<br>
<a class="learn-btn" href="/boolean-expressions/">View Example</a>
<a class="learn-btn" href="#">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
if (score > 50 && alive){
 win();
}
</pre>
</details>
</td>
</tr>

<tr>
<td>Input/Output</td>
<td>Handling data coming into the program (input) and displaying results back to the user (output).</td>
<td>
menus, controls
<br>
<a class="learn-btn" href="/input-output/">View Example</a>
<a class="learn-btn">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
console.log("Hello");
</pre>
</details>
</td>
</tr>

<tr>
<td>Keyboard Input</td>
<td>Detecting user key presses to control movement, actions, and interactions within the game.</td>
<td>
movement controls
<br>
<a class="learn-btn" href="/keyboard-input/">View Example</a>
<a class="learn-btn">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
document.addEventListener("keydown", e=>{
 console.log(e.key);
});
</pre>
</details>
</td>
</tr>

<tr>
<td>Canvas Rendering</td>
<td>Using the HTML canvas to draw shapes, images, and animations that create the visual part of the game.</td>
<td>
game visuals
<br>
<a class="learn-btn" href="/canvas-rendering/">View Example</a>
<a class="learn-btn">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
ctx.fillRect(10,10,50,50);
</pre>
</details>
</td>
</tr>

<tr>
<td>GameEnv Configuration</td>
<td>Setting up and controlling global game settings like speed, difficulty, levels, and environment behavior.</td>
<td>
levels, settings
<br>
<a class="learn-btn" href="/gameenv-configuration/">View Example</a>
<a class="learn-btn">Preview Code</a>
<details><summary>Show Code</summary>
<pre>
GameEnv.speed = 2;
</pre>
</details>
</td>
</tr>

</table>
</div>


<script>
document.querySelectorAll(".learn-btn").forEach(btn=>{
 if(btn.textContent.includes("Preview Code")){
   btn.addEventListener("click", e=>{
     e.preventDefault();
     const details = btn.nextElementSibling;
     if(details && details.tagName === "DETAILS"){
       details.open = !details.open;
     }
   });
 }
});
</script>

{% capture challenge0 %}
CSSE Ocean Game
{% endcapture %}

{% capture code0 %}
import GameControl from '@assets/js/GameEnginev1.1/essentials/GameControl.js';
import GameLevelOcean from '@assets/js/projects/ocean/levels/GameLevelOcean.js';

export const gameLevelClasses = [GameLevelOcean];
export { GameControl };
{% endcapture %}

{% include runners/game.html
   runner_id="cs111-0"
   challenge=challenge0
   code=code0
   hide_edit="true"
   width="100%"
   height="500px"
%}

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