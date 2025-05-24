# EX-06 - Looping
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
#include <stdio.h>
int main() {
   int a,b,i;
   scanf("%d %d",&a,&b);
   if(a%2!=0)a+=1;
   for(i = a;i<=b;i+=2){
       printf("%d ",i);
   }
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/4dbeb728-4db2-4053-8c11-4c76468417bf)
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
#include <stdio.h>
int main() {
   int r,i,j;
   scanf("%d",&r);
   for(i = 0;i<r;i++){
       for(j = 0;j<r-i-1;j++){
           printf(" ");
       }
       for(j = 0;j<=i;j++){
           printf("* ");
           
       }
     printf("\n");
   }
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/b9e3232d-8719-4d07-86ca-94404e05c8c0)

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
#include <stdio.h>
void add(int a,int b);
void sub(int a,int b);
int main(){
    int m,n;
    scanf("%d %d",&m,&n);
    add(m,n);
    sub(m,n);
}
void add(int a,int b){
    printf("%d + %d = %d\n",a,b,a+b);
}
void sub(int x,int y){
    printf("%d - %d = %d\n",x,y,x-y);
}

```

## OUTPUT:

![image](https://github.com/user-attachments/assets/f1d37f98-d25e-4cb3-b629-f4273e5d1415)

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
#include <stdio.h>
void sod();
int main(){
    sod();
}
void sod(){
    int m,osum = 0,c = 0;
    scanf("%d",&m);
    int temp = m;
    while(temp>0){
        c++;
        temp/=10;
    }
    temp = m;
    for(int i=0;i<c;i++){
        int rem = temp%10;
        if(rem%2!=0) osum+=rem;
        temp/=10;
    }
    printf("The sum of the odd digits in the number %d is %d\n\n",m,osum);
    sod();
}

```

## OUTPUT:


![image](https://github.com/user-attachments/assets/026c0beb-c050-4d4e-bc39-56ef6342d13a)

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
#include <stdio.h>
void Fact();
int main(){
    Fact();
}
void Fact(){
    int N, fact = 1;
    scanf("%d",&N);
    for(int i=1;i<=N;i++) fact *= i;
    printf("%d! = %d\n\n",N,fact);
    Fact();
}

```

## OUTPUT:

![image](https://github.com/user-attachments/assets/80aa9ef4-f791-4959-a906-f2814c040ac7)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
