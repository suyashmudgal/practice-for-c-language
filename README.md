 Write a C program to print a block F using the hash (#), where the F has a height of six characters and width of five and four characters. And also print a very large 'C
 Write a C program to convert specified days into years, weeks and days.Note: Ignore leap year.
 Write a C program that accepts an employee's ID, total worked hours in a month and the amount he received per hour. Print the ID and salary (with two decimal places) of the employee for a particular month.Test Data :
 Write a C program that accepts 4 integers p, q, r, s from the user where q, r and s are positive and p is even. If q is greater than r and s is greater than p and if the sum of r and s is greater than the sum of p and q print "Correct values", otherwise print "Wrong values".
 Write a C program that reads 5 numbers and sums all odd values between them. Test Data :

 -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 
 /*Write a C program that reads three floating-point values and checks if it is possible to make a triangle with them.
 Determine the perimeter of the triangle if the given values are valid.
Test Data : */

#include <stdio.h>

int main(){

    float a, b, c, perimeter;
    printf("enter the value of a== ");
    scanf("%f", &a);
    printf("enter the value of b== ");
    scanf("%f", &b);
    printf("enter the value of c== ");
    scanf("%f", &c);
    if(a + b > c && a + c > b && b + c > a){
        printf("The perimeter of the triangle is %f", a + b + c);
    }
    else
    {
        printf("The triangle is not possible");
    }
    return 0;

}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Write a C program that reads two integers and checks whether they are multiplied or not.

#include <stdio.h>

int main() {
    int num1, num2;

    // Ask the user for two integers
    printf("Enter two integers: ");
    scanf("%d %d", &num1, &num2);

    // Check if one number is a multiple of the other
    if (num1 % num2 == 0) {
        printf("%d is a multiple of %d.\n", num1, num2);
    } 
    else if (num2 % num1 == 0) {
        printf("%d is a multiple of %d.\n", num2, num1);
    } 
    else {
        printf("Neither number is a multiple of the other.\n");
    }

    return 0;
}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
// Write a C program that reads 5 numbers and counts the number of positive numbers and negative numbers.

#include <stdio.h>

int main(){

    int num1, num2, num3, num4, num5;
    int positive = 0, negative = 0;

    printf("Enter 5 numbers: ");
    scanf("%d %d %d %d %d", &num1, &num2, &num3, &num4, &num5);

    if (num1 > 0)
    {
        positive++;
    }
    else
    {
        negative++;
    }

    if (num2 > 0)
    {
        positive++;
    }
    else
    {
        negative++;
    }

    if (num3 > 0)
    {
        positive++;
    }
    else
    {
        negative++;
    }

    if (num4 > 0)
    {
        positive++;
    }
    else
    {
        negative++;
    }

    if (num5 > 0)
    {
        positive++;
    }
    else
    {
        negative++;
    }

    printf("Number of positive numbers: %d\n", positive);
    printf("Number of negative numbers: %d\n", negative);


    return 0;    
}

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/* Write a C program to compute the sum of consecutive odd numbers from a given pair of integers.
Test Data :*/

#include <stdio.h>
int main(){

    int a,b;
    printf("enter the first and last integer :- ");
    scanf("%d%d",&a,&b);
    int sum=0;
    for(int i=a;i<=b;i++){
        if(i%2!=0){
            sum+=i;
        }
    }
    printf("%d",sum);
    return 0;

}

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/* Write a C program to check if two numbers in a pair are in ascending order or descending order.
Test Data :*/

#include <stdio.h>

int main(){

    int num1, num2;
    printf("enter the value of num1 :-");
    scanf("%d",&num1);
    printf("enter the value of num2 :-");
    scanf("%d",&num1);

    if(num1>num2){
        printf("num1 is greater than num2\n");
        printf("assending order ");
    }
    else{
        printf("num1 is less than num2\n");
        printf("descending order");
    }
    return 0;


}

#include<stdio.h>
int main(){

    int arr[5];
    printf("Enter value to be stored in array> ");
    scanf("%d", &arr[0]);

    if(arr[0] > arr[1] && arr[1] > arr[2] && arr[2] > arr[3] && arr[3] > arr[4]){
        printf("descending  order");
    }
    else{
        printf("ascending order");
    }
    return 0;


}

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
two way are there to solve it

/* Write a C program to read a password until it is valid. For wrong password print "Incorrect password" and for correct password print, "Correct password" and quit the program. The correct password is 1234.
Test Data :*/
#include <stdio.h>
int main(){

    int a = 1234;
    int b;
    while(1){
        scanf("%d",&b);
        if(b == a){
            printf("Correct password");
            break;
        }
        else
        printf("Incorrect password");
}

#include<stdio.h>
int main(){

    int a = 1234;
    int b;

    printf("enter the value of b ::-");
    scanf("%d",&b);
    if( a == b){
        
        printf("correct password");

    }
    else{
        printf("incorrect password");
    }
    return 0;

}

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

