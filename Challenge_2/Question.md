# Part 1: Repair the corruption in this spreadsheet!

The spreadsheet consists of rows of apparently-random numbers. To make sure the recovery process is on the right track, they need you to calculate the spreadsheet's checksum. For each row, determine the difference between the largest value and the smallest value; the checksum is the sum of all of these differences.

For example, given the following spreadsheet:

| Value 1 | Value 2 | Value 3 | etc. | 
| --- | --- | --- | --- |
| 5 | 1 | 9 | 5 |
| 7 | 5 | 3 |
| 2 | 4 | 6 | 8 |

- The first row's largest and smallest values are 9 and 1, and their difference is 8.
- The second row's largest and smallest values are 7 and 3, and their difference is 4.
- The third row's difference is 6.
- In this example, the spreadsheet's checksum would be 8 + 4 + 6 = 18.

**What is the checksum for the spreadsheet in your puzzle input?**

Send John your answer, upload your code to github, and move on to the second part.

# Part 2: Working out the evenly divisble numbers

Actually, the user that had the corrupted spreadsheet doesn't really care about the checksum (as he is a standard user, they just wants it to work). All the user wanted is some information about the evenly divisible values in the spreadsheet. Unfortunately, none of us are equipped for that kind of calculation!

The goal is to find the only two numbers in each row where one evenly divides the other - that is, where the result of the division operation is a whole number. They would like you to find those numbers on each line, divide them, and add up each line's result.

For example, given the following spreadsheet:

| Value 1 | Value 2 | Value 3 | etc. | 
| --- | --- | --- | --- |
| 5 | 9 | 2 | 8 |
| 9 | 4 | 7 | 3 |
| 3 | 8 | 6 | 5 |

- In the first row, the only two numbers that evenly divide are 8 and 2; the result of this division is 4.
- In the second row, the two numbers are 9 and 3; the result is 3.
- In the third row, the result is 2.
- In this example, the sum of the results would be 4 + 3 + 2 = 9.

**What is the total sum of each row's result from the tsv spreadsheet?**

Send John your answer and update your code in gitbhub.

Challenge 2 is completed! Well Done!
