---
layout: post
codemirror: true
title: CSSE Objectives
description: A JavaScript game project demonstrating core Computer Science concepts including Object-Oriented Programming, inheritance, control structures, data types, and API integration. Built using a custom game engine, it features interactive gameplay, Canvas rendering, keyboard input, and state management. The project follows software engineering practices such as version control, debugging, testing, and documentation, and is aligned with CS111 learning objectives.
permalink: /information-checklist

---


<style>
  .table-container{
    width:100%;
    overflow-x:auto;
    background:#0d0d0d;
    padding:25px;
    border-radius:12px;
  }

  table{
    width:100%;
    border-collapse:collapse;
    background:#111;
    border:2px solid #f52bc9;
    box-shadow:0 0 12px rgba(98, 5, 67, 0.3);
    font-family: Arial, Helvetica, sans-serif;
  }

  th{
    background:#1a1a1a;
    color:#d9d9d9;
    font-size:24px;
    text-align:left;
    padding:20px;
    border:1px solid #ef2b9a;
  }

  td{
    padding:18px;
    border:1px solid #f02bc5;
    vertical-align:top;
    font-size:18px;
    line-height:1.5;
    color:#cfcfcf;
  }

  tr:nth-child(even){
    background:#161616;
  }

  tr:hover{
    background:#1f1f1f;
    transition:0.2s;
  }

  .objective{
    font-weight:bold;
    color:white;
    width:25%;
  }

  .meaning{
    width:35%;
  }

  .applied{
    width:40%;
  }

  .code{
    background:#2a2a2a;
    padding:3px 8px;
    border-radius:6px;
    color:#ffffff;
    font-family: Consolas, monospace;
  }
</style>

<div class="table-container">
  <table>

    <tr>
      <th>Learning Objective</th>
      <th>What It Means</th>
      <th>How It’s Applied</th>
    </tr>

    <tr>
      <td class="objective">Object-Oriented Programming</td>
      <td class="meaning">Organizing code using classes and objects.</td>
      <td class="applied">Used to create game characters, enemies, and reusable systems.</td>
    </tr>

    <tr>
      <td class="objective">Writing Classes</td>
      <td class="meaning">Creating blueprints for objects with properties and methods.</td>
      <td class="applied">Create classes like <span class="code">Player</span> and <span class="code">Enemy</span>.</td>
    </tr>

    <tr>
      <td class="objective">Methods & Parameters</td>
      <td class="meaning">Functions inside classes that can accept data.</td>
      <td class="applied">Example: <span class="code">move(direction, speed)</span></td>
    </tr>

    <tr>
      <td class="objective">Instantiation & Objects</td>
      <td class="meaning">Creating usable objects from classes.</td>
      <td class="applied">Example: <span class="code">const player = new Player()</span></td>
    </tr>

    <tr>
      <td class="objective">Inheritance (Basic)</td>
      <td class="meaning">One class can inherit features from another class.</td>
      <td class="applied">Example: <span class="code">class Enemy extends Character</span></td>
    </tr>

    <tr>
      <td class="objective">Method Overriding</td>
      <td class="meaning">Replacing a parent class method with a custom version.</td>
      <td class="applied">Override <span class="code">update()</span> or <span class="code">draw()</span>.</td>
    </tr>

    <tr>
      <td class="objective">Constructor Chaining</td>
      <td class="meaning">Using parent constructors inside child classes.</td>
      <td class="applied">Example: <span class="code">super(data)</span></td>
    </tr>

    <tr>
      <td class="objective">Control Structures</td>
      <td class="meaning">Logic that controls program flow.</td>
      <td class="applied">Used with loops and conditional statements.</td>
    </tr>

    <tr>
      <td class="objective">Iteration</td>
      <td class="meaning">Repeating code using loops.</td>
      <td class="applied">Example: <span class="code">for</span> and <span class="code">while</span> loops.</td>
    </tr>

    <tr>
      <td class="objective">Conditionals</td>
      <td class="meaning">Running code only if conditions are true.</td>
      <td class="applied">Example: <span class="code">if (health <= 0)</span></td>
    </tr>

    <tr>
      <td class="objective">Nested Conditions</td>
      <td class="meaning">Conditions placed inside other conditions.</td>
      <td class="applied">Used for advanced game logic checks.</td>
    </tr>

    <tr>
      <td class="objective">Data Types</td>
      <td class="meaning">Different kinds of data used in programming.</td>
      <td class="applied">Includes numbers, strings, booleans, arrays, and objects.</td>
    </tr>

    <tr>
      <td class="objective">Numbers</td>
      <td class="meaning">Numeric values used in calculations.</td>
      <td class="applied">Used for score, speed, damage, and position values.</td>
    </tr>

    <tr>
      <td class="objective">Strings</td>
      <td class="meaning">Text values stored in code.</td>
      <td class="applied">Used for names, dialogue, and labels.</td>
    </tr>

    <tr>
      <td class="objective">Booleans</td>
      <td class="meaning">True or false values.</td>
      <td class="applied">Example: <span class="code">isAlive = true</span></td>
    </tr>

    <tr>
      <td class="objective">Arrays</td>
      <td class="meaning">Lists that store multiple values.</td>
      <td class="applied">Used to store enemies, bullets, or items.</td>
    </tr>
https://poway.instructure.com/profile/settings
    <tr>
      <td class="objective">Objects (JSON)</td>
      <td class="meaning">Structured data using key-value pairs.</td>
      <td class="applied">Used for game configuration and settings.</td>
    </tr>

    <tr>
      <td class="objective">Operators</td>
      <td class="meaning">Symbols used for calculations and comparisons.</td>
      <td class="applied">Examples: <span class="code">+</span>, <span class="code">-</span>, <span class="code">===</span></td>
    </tr>

    <tr>
      <td class="objective">Mathematical</td>
      <td class="meaning">Performing arithmetic calculations.</td>
      <td class="applied">Used for movement, collision, and scoring systems.</td>
    </tr>

    <tr>
      <td class="objective">String Operations</td>
      <td class="meaning">Manipulating and combining text.</td>
      <td class="applied">Example: <span class="code">"Score: " + points</span></td>
    </tr>

    <tr>
      <td class="objective">Boolean Expressions</td>
      <td class="meaning">Expressions that evaluate to true or false.</td>
      <td class="applied">Used in game decision-making logic.</td>
    </tr>

    <tr>
      <td class="objective">Input/Output</td>
      <td class="meaning">Receiving user input and displaying results.</td>
      <td class="applied">Used for controls, menus, and game feedback.</td>
    </tr>

    <tr>
      <td class="objective">Keyboard Input</td>
      <td class="meaning">Detecting keyboard interactions.</td>
      <td class="applied">Used for player movement and controls.</td>
    </tr>

    <tr>
      <td class="objective">Canvas Rendering</td>
      <td class="meaning">Drawing graphics onto the screen.</td>
      <td class="applied">Used to render game characters and backgrounds.</td>
    </tr>

    <tr>
      <td class="objective">GameEnv Configuration</td>
      <td class="meaning">Setting up the game environment and settings.</td>
      <td class="applied">Used to configure levels, objects, and gameplay values.</td>
    </tr>

  </table>
</div>