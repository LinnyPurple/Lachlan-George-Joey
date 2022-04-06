---
layout: default
title: Reference Guide
nav_order: 3
---

# Reference Guide
{: .no_toc }

On this page, you'll find some helpful reminders and tips about this programming language.

## Website
The website we will use to run sample Brainfuck codes is [https://copy.sh/brainfuck/] (https://copy.sh/brainfuck/)

## Symbols

`>` Move one cell to the right.

`<` Move one cell to the left.

`+` Increment the current cell by one.

`-` Decrement the current cell by one.

`.` Output the current cell's value to the console.

`,` Get the next character in the input and store it in the current cell.

`[` Signal the start of a loop.

`]` Signal the end of a loop.

## Simple Functions

`[-]` Set the value of the current cell to 0.

`[-<+>]` Add the current cell to the cell on the left. Current cell will be zeroed out in the process.

`[-<->]` Subtract the current cell from the cell on the left. Current cell will be zeroed out in the process.

## ASCII Table

When outputting to the console, the ASCII value of that number will be printed rather than the number itself. For example, if the value of the current cell is `48`, `0` will be printed to the console.

![ASKEE TABLE](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/ASKEE%20table.png?raw=true "ASCII Tabe")

## Cell Table

In this language, all values are stored in 30,000 "Cells". Each cell can hold any number between 0 and 255. The pointer is always pointing to one of these cells. Whichever cell the pointer is pointing at will be the one affected by an instruction.

![Memory dump](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/Memory%20dump.png?raw=true "memorydump")
