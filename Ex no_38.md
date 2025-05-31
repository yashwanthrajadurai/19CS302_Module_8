# # Task

# # Given a positive integer denoting , do the following:

# If  41<=n <=49 print the lowercase English word corresponding to the number (e.g., forty one for 41 , forty two for 42 etc.).
If n>49 print Greater than 49.
## Input Format

The first line contains a single integer, .

## Constraints

## Output Format

If  41<=n <=49 print the lowercase English word corresponding to the number (e.g., forty one for 4 , forty two for 42 etc.).
If n>49 print Greater than 49.
## Sample Input

41
## Sample Output

forty one

AIM:

To write a program to print the English word corresponding to the given number.

ALGORITHM:

Start.

Define a variables.

Write a program to print the English word corresponding to the given number.

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End.

PROGRAM:

#include <stdio.h>

int main() {

 int num;
 
 scanf("%d", &num);
 
 switch (num) {
 
 case 41: 

printf("forty one\n"); break;

 case 42: 

printf("forty two\n"); break;

 case 43: 

printf("forty three\n"); 

break;

 case 44: 

printf("forty four\n"); break;

 case 45: 

printf("forty five\n"); break;

 case 46: 

printf("forty six\n"); break;

 case 47: 

printf("forty seven\n"); 

break;

 case 48:

printf("forty eight\n"); 

break;

 case 49: 

printf("forty nine\n"); break;

 default: 

printf(" Greater than 49\n"); break;

 }
 
 return 0;

}

OUTPUT

![Screenshot 2025-05-26 163728](https://github.com/user-attachments/assets/6e7a8c43-53b1-45e6-85a3-2fb55198b1fe)

RESULT:

Thus, the program is executed and verified successfully
