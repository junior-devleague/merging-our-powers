---
author:
- Somewha7
title: 'Merging Our Powers'
type: Activity
---

Summary
=======

Activity to teach the construction of a mergesort. Part of the Sorting Algorithm Series

Objective
=========

The time has come. Dr. Monsoon has arrived, and he's ready to rumble. Heroes Inc. has sent out their best and brightest, but it's just not enough... Slowly but surely you're losing ground, and it seems like nothing can stop Dr. Monsoon's unrelenting advance. Everyone's tried their best, but it seems like this is the end... But wait! You've reached an epiphany -- As in a vision, you've dreamed up a new sort -- one more powerful than any you've seen before, save possibly the quicksort, and maybe -- just maybe -- it'll be enough to save the day. Can you flesh out this vision, and create it before it's too late? The clock is ticking...

Prerequisites
=============

-   Basic usage of Python REPL


Requirements
============

-   Shell terminal or Python IDE
-   The pernicious pressure of a time bomb ticking down

Desired Outcomes
================

-   An understanding of the mergesort algorithm, and the ability to construct a mergesort in Python based on your own understanding

Tasks
=====

1.   Define 2 functions -- one will be called something along the lines of sort or mergesort and will take in 1 list (inlist) as an argument, and one will be alled something like sort and will take in two lists as arguments (list1, list2). The merge function will be called within the mergesort function, and is used to better distribute the density of the code & avoid having to write the same (large) block of code twice.
####  Merge Function:
2.  Create a variable newList, and then set it equal to an empty list on the next line.
3.  Define 2 variables, i & j, and set both equal to 0. They will be used to iterate over the 2 lists you're using as input
4.  Create a while loop that will run *while* two conditions are true -- i is less than the length of list1, and j is less than the length of list2
5.  Inside of the while loop, compare the values of list1 at index i and list2 and index j. Append whichever value is lesser to your newList variable, and add move one spot down on that list (*HINT:* what are i and j for?)
6.  Not all lists are created equal. Often times there will be cases where there are several values in one list and not the other. Use 2 more while loops to iterate over each list and append whatever values are left to newList.
7.  Return the function as being equal to newList

####  Mergesort Function:
8.  Get the middlemost index value of the list, and save it as mid. (*HINT:* lists won't always have an even *length*. How can you round them to the nearest whole number?)
9.  Define 2 new lists as being equal to the left & right halves of the list. (*HINT:* you can use *colons* to get a *portion* of a list, for instance the *left* and *right* half, so long as you know what the middlemost index value is)
10.  Mergesorts are divide and conquer, which means that they're recursive. establish the *base case* for when the list does not need to be sorted any more (*HINT:* A list of 1 item is by definition sorted), and then recursively call the mergesort function so long as that base case is not met. After running the mergesort function, set list1/list2 as equal to newList. (*HINT:* the mergesort function only takes in one list, but you have two that you need to sort... Maybe define 2 separate recursive statements, but have them follow the same pattern?)
11.  Run the merge function on list1 & list2 (previous mergesort call on them sorts them), and return the mergesort function as being equal to the value returned by the merge function.
12. Create a list, run the mergesort on it (make sure create a variable and set it equal to the mergesort function), and print out the sorted list!
