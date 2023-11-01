# Multiplication-Table-Generator-in-C
C program to generate multiplication table within the specified lower and upper limits using the concepts of loops(for and nested loop)

/* 
   Multiplication Table Generator using the concepts of loops
   Author: Ann Maria Anil
   Date: 1st November,2023
   Description: This program generates a multiplication table
                within the specified lower and upper limits by 
				using the concepts of loops only
*/

#include<stdio.h>

int main()
{
    int lowerLimit, upperLimit;

    // Input lower limit from the user
    printf("Enter the lower limit: ");
    scanf("%d", &lowerLimit);

    // Input upper limit from the user
    printf("Enter the upper limit: ");
    scanf("%d", &upperLimit);

    // Display a horizontal line of numbers
    printf("\t");
    for (int number = lowerLimit; number <= upperLimit; number++)
	{
        printf("%d \t", number);
    }
    printf("\n");

    // Display a line of asterisks
    for (int i = lowerLimit; i <= upperLimit; i++)
    {
        printf("************************");
    }
    printf("\n");

    // Display a multiplication table with row and column headers
    for (int row = lowerLimit; row <= upperLimit; row++)
    {
        printf("%d * \t", row);
        for (int col = lowerLimit; col <= upperLimit; col++)
	    {
            int product = row * col;
            printf("%d \t", product);
        }
        printf("*\n");
    }

    // Display a line of asterisks
    for (int i = lowerLimit; i <= upperLimit; i++) 
	{
        printf("****************");
    }

    return 0; // Indicate successful program execution
}
