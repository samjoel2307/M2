# EX-06 - Looping

## NAME: R . NITHISH AADITIYAA

## REGISTER NO: 25011876 [ 212225040287 ] 

## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int N,M;
    scanf("%d %d",&N,&M);
    int itr;
    printf("Even numbers:");
    for(itr=N;itr<=M;itr++)
    {
        if(itr%2==0)
        {
            printf("%d ",itr);
        }
    }
    return 0;
}
```
## OUTPUT:



<img width="902" height="233" alt="Screenshot 2026-03-26 110635" src="https://github.com/user-attachments/assets/1580b5bf-aef8-4aa0-a59e-91e1104a9610" />



## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 
# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int row,col,N;
    scanf("%d",&N);
    for(row=1;row<=N;row++)
    {
        for(col=N;col>row;col--)
        {
            printf(" ");
        }
        for(col=N;col>N-row;col--)
        {
            printf("*");
        }
        for(col=row;col<row*2-1;col++)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}
```
## OUTPUT:

<img width="885" height="422" alt="Screenshot 2026-03-26 111455" src="https://github.com/user-attachments/assets/15ba7253-cc8b-47e6-898e-f2446aecffda" />



## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 
# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include<stdio.h>
void add(int n1,int n2)
{
    int add=n1+n2;
    printf("Addition of %d and %d is %d\n",n1,n2,add);
    return;
}
void sub(int n1,int n2)
{
    int sub=n1-n2;
    if(sub>=0)
    printf("Subtraction of %d and %d is %d",n1,n2,sub);
    else
    printf("Subtraction of %d and %d is %d",n1,n2,-1*sub);
    return;
}
int main()
{
    int num1,num2;
    scanf("%d %d",&num1,&num2);
    add(num1,num2);
    sub(num1,num2);
    return 0;
}
```
## OUTPUT:

<img width="904" height="259" alt="Screenshot 2026-03-26 111606" src="https://github.com/user-attachments/assets/b0784b3b-e3ef-4056-b60a-5e41cfaa9288" />


## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 
# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int n,dig,sum=0;
    scanf("%d",&n);
    int check=n;![alt text](image.png)
    for(int itr=n;n>0;n/=10)
    {
        dig=n%10;
        if(dig%2!=0)
        {
            sum+=dig;
        }
    }
    printf("Sum of odd digits of number %d is %d",check,sum);
    return 0;
}
```
## OUTPUT:

<img width="917" height="221" alt="Screenshot 2026-03-26 111803" src="https://github.com/user-attachments/assets/c94a3866-4379-494e-8551-e1fa7b64e3fe" />



## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.


# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include<stdio.h>
int fact(int num)
{
    int check=1;
    for(int itr=num;itr>0;itr--)
    {
        check*=itr;
    }
    return check;
}
int main()
{
    int num;
    scanf("%d",&num);
    printf("The factorial of %d is %d",num,fact(num));
    return 0;
}
```
## OUTPUT:

<img width="900" height="198" alt="Screenshot 2026-03-26 113258" src="https://github.com/user-attachments/assets/96019111-b570-4fa1-a932-0dc39e4358a8" />


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
