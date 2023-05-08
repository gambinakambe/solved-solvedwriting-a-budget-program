Download Link: https://assignmentchef.com/product/solved-solvedwriting-a-budget-program
<br>
In this project you will write a budget program. The project has been divided in multiple steps to make it easier to implement.

Input Files

The program will use two input files: budget.txt and expense.txt.

budget.txt – Budget FileIt is a file that contains the expense type and the maximum expense allowed for this type. The Budget Type and the MaxAmount are separated by coma characters and are between quotes. The Budget file contains the following fields: “ExpenseType” ­ This is the expense type, such as MEALS, SCHOOL etc “MaxAmount” ­ This is the maximum amount that has been allocated to this expense.

expenses.txt – Expenses File

It is a file that contains the expense entries, one expense for each line. This is a file that very likely you can obtain from your bank account web page. The format of each line is the following: The goal of this project is to read the budget.txt and expense.txt files, determine how much money has been spent in a specific expense type and tell you if there is an over budget.Step 1. How To Read the budget.txt fileFor reading the budget.txt file we give you the following example code of the program budget.py. It is important that you understand well this code since it will help you write the other parts of the program. The function readBudget reads all the lines of the file and puts them in a list called lines. It uses the function lines[i].split(“,”)to split the line into multiple fields and stores it in list. It then extracts the expense type exptype and max amount maxamount from the line and strips them from any quotes and $ sign. It then creates a dictionary entry with the fields exptype and maxamount that is added to the list budget that contains all the budget entries. The function printBudget iterates over all the budget entries and prints them in a nice format. It uses “$%0.2f” % num for formatting of the decimals and it uses ljust and rjust form alignment. This is an example of the output:

Step 2Write a program readExpense.py that it will read the expenses.txt file and it will print the expenses in a table similar to what was printed in step 1. We suggest you to write a function that reads the expenses and a function that prints the expenses. Use as base the code in budget.py. The Main() program is called only when readExpense.py is run directly and not when it is imported from another file.

Step 3Write a program called expenseByType.py that it will print the total of the expenses by type. It will read both the expense.txt file and the budget.txt file and it will print the total for each expense type. The

Step 4Draw an expense pie chart like the following one that shows the expenses as a percentage of the total. Only use the graphics.py library. Hint: Draw lines of different colors from the center of the screen (0,0) to the edges of the circle (R*cos(2*pi*i/n),R(sin(2*pi*i/n)) where n is the total number of lines and I goes from 0 to n. Change the color of the lie according to the percentage displayed.