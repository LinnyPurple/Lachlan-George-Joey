---
layout: default
title: Print Numbers Program
parent: Tutorials
nav_order: 1
---

# Print Number Program
{: .no_toc }

A basic printing program gives the user the ability to manipulate the cells' contents and output their values. This program allows the user to print the numbers 1 to 10.

We will enter all the commands and codes into the input box:
![inputbox](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/inputbox.png?raw=true"inputbox")

## Step 1 - Moving the Cell:
The way we plan on printing out numbers is to print out each individual character by using counters and a loop.

First, we need to move cells and initialize counters for the loop.

1. We start by updating the cell's value from 0 to 49, the ASCII character `1`. We do this by typing the `+` 49 times.  
`+++++++++++++++++++++++++++++++++++++++++++++++++`  
The `+` allows us to increment the cell's value by 1.  
Now we need to get the program to input a `\n`, which allows the program to print each number on a new line.
2. Type `>` followed by 10 `+`.  
`>++++++++++`  
After the new line, we will need to initialize the counters.  
3. Type `>` followed by 9 `+`.  
`>+++++++++`  
This will allow us to assign Cell 2 to 9 as counters.  

At the end of the step 1 you should have something like this in the input box:
![step1](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/step1.png?raw=true"step1")

## Step 2 - The Loop
We will now create a loop that allows us to print numbers from 1 to 9.

We first start the loop by using the `[` operator:

1. Type `[` into the input box.  
`[`  
Since we are aiming to print in ascending order we need to move the data pointer to the beginning.  
2. Enter `<<` into the input box.  
`<<`  
This moves the data pointer to cell 0.  
We start by printing cell 0, which is has `1` assigned to it.  
3. Enter `.` followed by `+` into the input box.  
`.+`  
This prints 1 then increments cell 0.  
Now we have to move the data pointer to cell 1, which has `\n` assigned to it and invoke the new line function.  
4. Type `>` followed by `.` into the input box.  
`>.`  
This moves the pointer to cell 1 and then prints a new line.  
We move the the data pointer to cell 2, which has `9` assigned to the cell and will act as a counter.  
5. Enter `>` followed by `-` into the input box.  
`>-`  
Now we end the loop by using the closing square bracket.  
6. Type `]` into the input box.  
`]`  
This loop will use the counter `9` we have assigned earlier and loop until the counter reaches 0.  

At end of this step, you should have something like this:
![step2](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/step2.png?raw=true"step2")

## Step 3 - Resetting the counter
The memory used to activate the counter in the previous step would need to cleared. This step is to make sure no extra memory is being wasted.

We first begin by setting cell 2 to 9.

1. Type in `+` 9 times into the input box.  
`+++++++++`  
Like the previous step, we use a loop to avoid redundant operations.  
2. Enter `[` into the input box.  
`[`  
This operator lets us start a loop.  
Then, we move the data pointer to cell 0 and decrease the value.  
3. Enter `<<` followed by `-`.  
`<<-`  
Now, we need to move the pointer to cell 2 where we can locate the counter.  
4. Enter `>>` followed by `-`.  
`>>-`  
This will move the pointer to cell 2 and decrease the counter.  
Finally, we close off the loop by using the closing square bracket.  
5. Enter the `]` to close off the loop.  
`]`  
This loop will decrease the counter from `9` to `0`.

At the end of this step you should have something like this.
![step3](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/step3.png?raw=true"step3")

## Step 4 - Print 10
The loop from step 2 prints the numbers 1 to 9. Our goal in this program is to also include '10' as well. Since we only need to print one number, we do not need a loop.

Remember how we assigned `1` to a cell? We can avoid redundancy and use what we currently have.

First, we move the data pointer to cell 0 where we stored the value `1`.

1. Type `<<` into the input box.  
`<<.`  
This operation allows us to print `1` which is the first half of `10`.  
Now we decrease the value in cell 0 (which is `1`) and print.  
2. Type `-` followed by `.` into the input box.  
`-.`  
This allows us to print the second of `10` and complete the program.  
We can finish the program by printing the last `\n` to improve clarity and readability.  
3. Enter `>` followed by `.` to generate a new line.  
`>.`  
This moves the data pointer to cell 1 where we find `\n` and prints a new line.  
4. Now we can finish the the program by clicking the run button.  
![run](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/run%20button.png?raw=true"run")

## Final Program
The finished program should look something like this:
```
This program prints numbers 1 to 10 to the console

+++++++++++++++++++++++++++++++++++++++++++++++++  Assigning '1' to Cell 0
>++++++++++  Assigning '\n' to cell 1
>+++++++++  This assigns the value '9' to cell 2 which we will use as counter later on
[  Print numbers 1 to 9
<<  Data pointer to cell 0
.+  Print and increment cell 0
>.  Data pointer to cell 1 and print the newline
>-  Data pointer to cell 2 and decrement counter
]  Loop till counter is 0
+++++++++  Set cell 2 to 9
[  Set cell 0 to '1'
<<-  Data pointer to cell 0 and decrement
>>-  Data pointer to cell 2 and decrement counter
]  Loop till counter is 0
<<.  Data pointer to cell 0 and print '1'
-.   Decrement cell 0 and print '0'
>.   Data pointer to cell 1 and print newline
```
![output](https://github.com/LinnyPurple/Lachlan-George-Joey/blob/gh-pages/assets/images/output.png?raw=true"output")

## Conclusion
Congratulations! You have printed a series of numbers.
