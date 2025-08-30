
# CISC 4080 lab1

## Goal:

1. Get familiar with Python programming,
2. practice using basic data structures in Pyton: list,
3. practice implementing a few basic algorithms as Python functions, and
4. practice reading files 
   
## Preparation

1. Download Python (  Python 3.10, 3.11, or 3.12 or higher) 

(Xiang: can you find good resources for Windows and Mac users?)

2. A crash course: Python for C++ Programmers 

'''
https://python.pages.doc.ic.ac.uk/cpp/lessons/cpp/01-intro/index.html
'''

Feel free to go back to the course for more examples at your convenience. 

3. Download this data file which contains random integers.
   
## Program Execution:

The following example illustrates how your program should work.

1. Your program should open the given data file,  read integers from the file and store them in a list.

2. The program then prompts the user to enter a number to search for, and then performs linear search in the list and reports all occurrences of the number, e.g., if the number appears in position 3, 20, 81, the function should return a list, containing indices [3, 20, 81]. 

3.  The program then sorts the list using the selection sort function that you implement.

4.  The program then performs binary search, using the same number as in step 2, and display **any** occurrence if the number appears multiple times in the list.
    **Extra credits**: Extend binary search so that it returns the range of indices where the target number appears, for example, in sorted list [2, 3, 3, 3, 7, 9], if we search for 3, binary search can return [1,3] (as L[1…3] all contains 3). 

5.  Reload the file into a new list, and call the Python’s built-in sorting function 

6.  Output the running time of linear search and binary search, and the running time of selection sort and Python’s built-in sorting function. 


```
   $ python3.10 lab1.py
   Read input from data.txt ...
   Enter a number to seearch for: 5
   5 appears in positions 4, 10, 31 
   Sorting the data with selection sort ...
   Binary search for 5 in sorted list... 
   5 appears in position 14
   Sorting the data using Python's built-in sort function....
   Running time comparison result:
   linear search: 0.003 seconds
   binary search: 0.0004 seconds
   selection sort: 0.4 seconds
   built in sort:  0.32 seconds
```

## Detail Requirements:
1. Please name your program as **lab1.py**.
2. Please define functions for 
   * Reading integers from file and return them as a list
   * Linear search
   * Selection sort
   * Binary search
3. Comment all your functions with a function header, describing their functionalities, param, pre-condition and post-condition (see the slides for example)
4. At the top of your Python code, have a block of comments describing the purpose of the lab, author, last modification time, known bugs…   


## Submission

Submit your code in C++, named **lab1.py** on Blackboard. 


## Grading:

Automatic test cases (50 pts): 5 test cases each tests one of the sorting functions. 
For this to work, pay attention to the following details:

1. The command used in your program needs to match with those specified in this description, i.e., **selection**, **rselection**, **bubble**, **rbubble**
2. Before submitting your program, comment out or delete any cout statements except for the one that displays the vector after sorting function is called.

Handgrading (20 pts): style, comment, and logic...
See the autograder page for this project for details.

