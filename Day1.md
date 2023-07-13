# Day 1: Introduction To Apex | DataType | Collection | Conditional Statements

This README file summarizes the key concepts covered on Day 1 of my learning journey. On this day, I explored the fundamentals of Apex, including an introduction to the language, values & data types, and operators. I also solved the Assignment code.

## Lesson Summary
On Day 1 of our training, we focused on the following key concepts:

- Introduction to Apex: We started by understanding what Apex is and its role within the Salesforce ecosystem.

- Data Types in Apex: We explored the different data types available in Apex, such as integers, strings, booleans, and more.

- Variables in Apex: We learned how to declare and use variables to store and manipulate data in Apex.

- Operators: We discussed various operators in Apex, including arithmetic, comparison, and logical operators.

- Collections in Apex: We explored collections, such as lists and maps, and learned how to store and retrieve data from them.

- Conditional Statements in Apex: We covered conditional statements like if-else statements, switch statements, and the ternary operator.

- Assignment: We completed a coding exercise to calculate the sum of even numbers in a list.

## Assignment: Sum of Even Numbers
Write an Apex program to store all the numbers in a List starting from 1 until 20. Only numbers stored at even positions in the List should be added to get their sum, which should be output to the Debug Log.

### Solution
Here is the code solution to the assignment:

```apex
integer TotalSumEven = 0;
list <integer> listOfNumbers = new list <integer>();

for(integer i = 1 ; i <= 20 ; i++ )
{
   listOfNumbers.add(i);
}

system.debug('listOfNumbers: '+listOfNumbers);

for(integer i = 1 ; i < listOfNumbers.size(); i++ )
{
   if(Math.mod(listOfNumbers[i], 2) == 0)
   {
        TotalSumEven += listOfNumbers[i];
   }
}

system.debug('The total sum of even numbers from [1, 20] is: '+TotalSumEven);
```
Feel free to explore the code snippets and solutions provided for the assignment. 

I hope you had a productive Day 1, and I encourage you to continue building upon these concepts in your Salesforce backend training. Keep up the great work!

Happy coding! 🎉
