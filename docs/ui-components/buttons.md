---
layout: default
title: Addition Program
parent: Tutorials
nav_order: 2
---

# Simple Addition Program
{: .no_toc }

An addition program is one of the simplest ways to use a user's input in a program. In this example, the user will input two numbers, and the program will print the sum of them.

## Step 1
Before we can add numbers, we need to get the numbers we're going to add! To get user input in Brainfuck, the ',' character is used. Each time it is used, it will get the next character in the input and set the current cell to the ASCII value of that character.

For this program, the input will be formatted as `# #` with '#' being replaced by a number from 1-9.

Getting the first number is easy, we just need to do a single ','. Then we need to move to the next cell and store the second number. The numbers are separated by a space character so we will need to do ',,' to get it.

Which means our first few lines are going to look like this:
```
,>
,,
```
