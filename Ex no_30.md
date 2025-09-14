# EX 30 C program to add two integer elements in an array using realloc() and that array already has three elements.
## DATE:
## AIM:
To write a C program to add two integer elements in an array using realloc() and that array already has three elements.

## Algorithm
1. Start.
2. Declare array size
3. Initialize array elements using malloc()
4.  Update array size using realloc()
5. Print the result.
6. End.  

## Program:
```
/*
C program to add two integer elements in an array using realloc() and that array already has three elements.

Developed by: SRINIVASAN V
RegisterNumber: 212222043008  
*/
```
```
#include <stdio.h>
#include <stdlib.h>
int main() {
 int *arr, size, i;
 size = 3;
 arr = (int *)malloc(size * sizeof(int)); 
 for (i = 0; i < size; i++) {
 arr[i] = i * 10; }
 printf("Original array:\n");
 for (i = 0; i < size; i++) {
 printf("%d ", arr[i]);
 }
 printf("\n");
 size *= 2;
 arr = (int *)realloc(arr, size * sizeof(int)); 
 for (i = size / 2; i < size; i++) {
 arr[i] = i * 10;
printf("Updated array:\n");
 for (i = 0; i < size; i++) {
 printf("%d ", arr[i]);
 }}
```
## Output:

<img width="458" height="233" alt="438875097-aa2e0ad2-10f1-4c1b-b022-9b385ecd3b47" src="https://github.com/user-attachments/assets/18152bd3-ebd2-4d98-a07f-4f8797ff6bac" />

## Result:
Thus the program was executed and the output was verified successfully.
