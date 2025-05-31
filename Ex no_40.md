## Given an array of strings sorted in lexicographical order, print all of its permutations in strict lexicographical order. If two permutations look the same, only print one of them. See the 'note' below for an example.

Complete the function next_permutation which generates the permutations in the described order.

## For example, s=[ab,bc,cd]. The six permutations in correct order are:

ab bc cd
ab cd bc
bc ab cd
bc cd ab
cd ab bc
cd bc ab
Note: There may be two or more of the same string as elements of .
## For example, s=[ab,bc,cd]. Only one instance of a permutation where all elements match should be printed. In other words, if s[0]==s[1], then print either s[0]  or s[1] but not both.

A three element array having three distinct elements has six permutations as shown above. In this case, there are three matching pairs of permutations where ab and ba are switched. We only print the three visibly unique permutations:

ab ab bc
ab bc ab
bc ab ab
## Input Format

The first line of each test file contains a single integer , the length of the string array .

Each of the next  lines contains a string .

Constraints

 contains only lowercase English letters.
Output Format

Print each permutation as a list of space-separated strings on a single line.

## Sample Input 0

2
ab
cd
## Sample Output 0

ab cd
cd ab
## Sample Input 1

3
a
bc
bc
## Sample Output 1

a bc bc
bc a bc
bc bc a

AIM:

To write a program to print permutation for the given string.

ALGORITHM:

Start.

Define a variables.

Write a program to print permutation for the given string.

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End.

PROGRAM:

#include <stdio.h>

#include <string.h>

void swap(char *x, 

char *y) {

 char temp;
 
 temp = *x;
 *x = *y;
 
 *y = temp;

}

void permute(char *str, 

int l, int r) {

 
 if (l == r) {
 
 printf("%s\n", str);
 
 } else {
 
 for (int i = l; i <= 

r; i++) {

 swap((str + l), 

(str + i)); 

 permute(str, l + 

1, r); 

 swap((str + l), 

(str + i)); 

 }
 
 }

}

int main() {

 char str[100];

printf("Enter a 

string: ");

 scanf("%s", str);
 
 int n = strlen(str);
 
 printf("All 

permutations of the 

string are:\n");

 permute(str, 0, n - 1);

 
 return 0;

}

OUTPUT

input

![Screenshot 2025-05-26 164427](https://github.com/user-attachments/assets/ec4233d5-8e7c-4b37-8ef6-6558c2941fb8)

output

![Screenshot 2025-05-26 164457](https://github.com/user-attachments/assets/58cbc181-23c4-4503-9b37-d895be9d2538)

RESULT:

Thus, the program is executed and verified successfully.
