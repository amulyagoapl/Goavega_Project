# Goavega_Project
Brief explanation of my approach:
Time Range Expander (Command Line Application)

 Overview
This Python command line application accepts a compact time range expression as input and expands it into all individual integer values expressed by that input.

The input can contain:
- Individual values 
- Ranges using "-"
- Comma-separated combinations of values and ranges (`9-12,14,16-18`)

The application prints out all expanded values in ascending order, separated by spaces.


Approach Explanation

1. Read the input string from the command line arguments using "sys.argv".
2. Split the input string by commas to process each segment separately.
3. For each segment:
   - If it contains "-", it is a range expression:
     - Split the segment into start and end values
     - Convert them to integers
     - Expand all values from start to end (Don't include)
   - Otherwise, it is an individual integer value.
4. Store all numbers in a list.
5. Sort the list to print in ascending order.
6. Print the final result as a space-separated string.

Setup Instructions

- Python 3.x is installed on your computer

To verify Python is installed:
bash
python --version
