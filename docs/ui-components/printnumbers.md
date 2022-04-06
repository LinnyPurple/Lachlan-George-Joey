---
layout: default
title: Print Numbers Program
parent: Tutorials
nav_order: 1
---

# Print Number Program
{: .no_toc }

A basic printing program gives the user the ability to manipulate the contents of the cells and output their values. This program allows the user to print numbers 1 to 10 in a loop.

## Step 1 - Moving the Cell:
The way we plan on printing out numbers is to print out each character individually by using counters and a loop.

First, we need to move Cells and intialize counters for the loop.

1. We start by moving the Cell from 0 to `1`. We do this by typing the `+` 49 times  
`+++++++++++++++++++++++++++++++++++++++++++++++++`  
The `+` allows us to move the cell.  
Now we need to get the program to input a `\n`, which allows the program to print each number on a new line.
2. Type `>` followed by 10 `+`  
`>++++++++++`  
After the new line, we will need to initialize the counters.  
3. Type `>` followed by 9 `+`  
`>+++++++++`  
This will allow us to assign Cell 2 to 9 as counters.  


## Step 2 - The Loop:
We will now create a loop that allow us to print numbers from 1 to 9.

We first start the loop by using the operator:

1. Type `[` into the input box.  
`[`  
Since we are aiming to print in a ascending order we need to move the data pointer to the begining.  
2. Enter `<<` into the input box.  
`<<`  
This moves the data pointer to cell 0  
We start by printing cell 0, which is has `1` assigned to it.  
3. Enter `.` followed by `+` into the input box  
`.+`  
This prints 1 then increments cell 0.  
Now we have to move the data pointer to cell 1, which has `\n` assigned to it and invoke the new line function.  
4. Type `>` followed by `.` into the input box  
`>.`  
This moves the pointer to cell 1 and then prints a new line.  
Lastly, we move the the data pointer to cell 2, which has `9` assigned to the cell and will act as a counter.  
5. Enter `>` followed by `-` into the input box.  
`>-`  
Now we end the loop by simply using the closing square bracket.  
6. Type `]` into the input box.  
`]`  
This loop will utilize the counter `9` we have assigned earlier and loop until the counter reaches 0.  


## Step 3 - Resetting the counter
The memory used to activate the counter in the previous step would need to cleared. This step is to make sure no extra memories are being waster.

We first begin by setting cell 2 to 9.

1. Type in `+` 9 times into the input box.  
`+++++++++`  
Like the previous step, we utilize a loop to avoid redundant operations.  
2. Enter `[` into the input box.  
`[`  
This operator lets us start a loop.  
Then, we move the data pointer to cell 0 and decrease the value.  
`<<-`  
Now, wee need to move the pointer to cell 2 where the counter is located.  
`>>-`  
This will move the pointer to cell 2 and decrease the counter.  
Finally, we close off the loop by using the closing square bracket.  
`]`  
This loop will ultimately decrease the counter from `9` to `0`.

## Step 4 - Print the rest of the number
The loop from step 2 prints number 1 to 9. Our goal in this program is to include '10' as well. Since only one number is required to print, we do not need a loop.

Remember how we have assigned `1` to a cell? we can avoid redundancy and use what we currently have.

Firstly, we move the data point to cell 0 where the `1` is located.

`<<.`

This operation allows us to print `1` which is the first half of `10`.

Now we decrease the value in cell 0 (which is `1`) and print.

`-.`

This allows us to print the second of `10` and complete the program. 

We can finish off the program by printing the last `new line` to improve clarity and readability

`>.`

This moves the data pointer to cell 1 where `\n` is located and prints a new line.

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

## Conclusion
Congratulation !! You have just printed a series of number.
