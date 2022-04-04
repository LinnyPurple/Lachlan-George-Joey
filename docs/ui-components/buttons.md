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
Before we can add numbers, we need to get the numbers we're going to add! To get user input in Brainfuck, the `,` character is used. Each time it is used, it will get the next character in the input and set the current cell to the ASCII value of that character.

For this program, the input will be formatted as `# #` with '#' being replaced by a number from 1-9.

Getting the first number is easy, we just need to do a single `,`. Then we need to move to the next cell and store the second number. The numbers are separated by a space character so we will need to do `,,` to get it.

Which means our first few lines are going to look like this:
```
,>
,,
```

## Step 2
Now, we need to add both numbers together. To add cells together, we are going to use a loop. A loop will do a set of commands until the cell it's at at the start of an iteration is equal to 0. Loops are started with `[` and end with `]`. An adding loop will look something like this:

```
[-<+>]
```

This loop starts at cell 1, which is where the second number from the input is. It will subtract one from cell 1, move to cell 0, add one to cell 0, then move back to cell 1. When cell 1 reaches zero, the loop will end and the program will move on to the next set of instructions.

