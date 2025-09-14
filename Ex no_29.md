# EX 29 C program to create two float variables using calloc() and find minimum among them.
## DATE:
## AIM:
To write a C program to create two float variables using calloc() and find minimum among them.

## Algorithm
1. Start.
2. Initialize two variables value of calloc().
3. Prompt the user to enter values.
4. Read the values using scanf.
5. Find minimum and print result
6. End

## Program:
```
/*
C program to create two float variables using calloc() and find minimum among them.
Developed by: SRINIVASAN V
RegisterNumber: 212222043008 
*/
```
```
#include <stdio.h>
#include <stdlib.h>
int main() {
 int *num1, *num2, minimum;
 num1 = (int *)calloc(1, sizeof(int));
 num2 = (int *)calloc(1, sizeof(int));
 num1= 5.8 , num2 = 6.5;
 minimum = (*num1 < *num2) ? *num1 : *num2;
 printf("%d\n", minimum);
 free(num1);
 free(num2);
```

## Output:

<img width="627" height="295" alt="439186717-9964ef99-9116-4486-8e09-5dc3c9c094cd" src="https://github.com/user-attachments/assets/20a7caa7-0983-4ec5-a94b-b8493e48b5f7" />



## Result:
Thus the program was executed and the output was verified successfully.
