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

/* Write a C program that reads 5 numbers, counts the number of positive numbers, and prints out the average of all positive values.*/

#include <stdio.h>
int main() {

    float numbers[5], total=0, avg; // Declare an array to store 5 numbers, and variables for total and average
    int j, pctr=0; // Declare variables for loop counter and positive count

    // Prompt user for five numbers and store them in the array
    printf("\nInput the first number: "); 
    scanf("%f", &numbers[0]);
    printf("\nInput the second number: "); 
    scanf("%f", &numbers[1]);
    printf("\nInput the third number: "); 
    scanf("%f", &numbers[2]);
    printf("\nInput the fourth number: "); 
    scanf("%f", &numbers[3]);
    printf("\nInput the fifth number: "); 
    scanf("%f", &numbers[4]);

    for(j = 0; j < 5; j++) {
        if(numbers[j] > 0) // Check if the number is positive
        {
            pctr++; // Increment positive count
            total += numbers[j]; // Add positive number to total
        }   
    }

    avg = total/pctr; // Calculate average of positive numbers

    // Print the counts of positive numbers and the average
    printf("\nNumber of positive numbers: %d", pctr);
    printf("\nAverage value of the said positive numbers: %.2f", avg);
    printf("\n");

    return 0;
}

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/* Write a C program to check whether a given integer
 is positive even, negative even, positive odd or negative odd. 
Print even if the number is 0.
*/
#include <stdio.h>

int main(){

    int num;

    printf("enter the number :");
    scanf("%d", &num);

    if(num > 0){
        if(num % 2 == 0){
            printf("positive even");
        }
        else{
            printf("positive odd");
        }
    }
    else if(num < 0){
        if(num % 2 == 0){
            printf("negative even");
        }
        else{
            printf("negative odd");
        }
    }
    else{
        printf("number is zero");
    }
    return 0;
    
}

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/* Write a C program to print all numbers between 1 and 100 
which are divided by a specified number and the remainder will be 3.*/
#include <stdio.h>

int main()
{

    int n;
    printf("enter the number :");
    scanf("%d", &n);
    for (int i = 1; i <= 100; i++)
    {
        if (i % n == 3)
        {
            printf("%d ", i);
        }
    }
    return 0;
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Write a C program that accepts some integers from the user and finds the highest value and the input position. */
#include <stdio.h>

int main() {

    int a, b, c, d;
    int highest, position;

    printf("Enter the 4 numbers: ");
    scanf("%d %d %d %d", &a, &b, &c, &d);

    // Initialize highest with the first number and position with 1
    highest = a;
    position = 1;

    // Compare with second number
    if (b > highest) {
        highest = b;
        position = 2;
    }
    
    // Compare with third number
    if (c > highest) {
        highest = c;
        position = 3;
    }
    
    // Compare with fourth number
    if (d > highest) {
        highest = d;
        position = 4;
    }

    printf("The highest number is: %d\n", highest);
    printf("The position of the highest number is: %d\n", position);

    return 0;
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/*37. Write a C program to read the coordinates (x, y) (in the Cartesian system) and find the quadrant to which it belongs (Quadrant -I, Quadrant -II, Quadrant -III, Quadrant -IV).
Note: A Cartesian coordinate system is a coordinate system that specifies each point uniquely in a plane by a pair of numerical coordinates.
These are often numbered from 1st to 4th and denoted by Roman numerals: I (where the signs of the (x,y) coordinates are I(+,+), II (−,+), III (−,−), and IV (+,−).*/

#include <stdio.h>

int main()
{

    float x, y;
    printf("enter the value of x and y : ");
    scanf("%f %f", &x, &y);

    if (x > 0 && y > 0)
    {
        printf("quadrant -I");


    }
    else if (x < 0 && y > 0)
    {
        printf("quadrant -II");
    }
    else if (x < 0 && y < 0)
    {
        printf("quadrant -III");
    }
    else
    {
        printf("quadrant -IV");
    }
    return 0;
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/*38. Write a program that reads two numbers and divides the first number by the second number.
 If division is not possible print "Division is not possible".
*/

#include <stdio.h>

int main()
{

    int a, b;

    printf("enter the first number :");
    scanf("%d", &a);

    printf("enter the second number :");
    scanf("%d", &b);

    if (b == 0)
    {
        printf("division is not possible");
    }
    else
    {
        printf("answer is %d", a / b);
    }

    return 0;
    }
    
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

/*3
9. Write a C program to calculate the sum of all numbers not divisible by 17 between 
two given integer numbers.
*/

#include <stdio.h>

int main()
{

    int a, b;

    printf("enter the first number : ");
    scanf("%d", &a);

    printf("enter the second number : ");
    scanf("%d", &b);

    while (a % 17 != 0 || b % 17 != 0)
    {
        if (a % 17 != 0)
        {
            a = a + 1;
        }
        if (b % 17 != 0)
        {
            b = b + 1;
        }
    }

    int sum = a + b;

    printf("sum is : %d", sum);

    return 0;
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/*40. Write a C program that finds all integer numbers that divide by 7 and
 have a remainder of 2 or 3 between two given integers.
*/

#include <stdio.h>

int main() {

    int i, j;

    printf("Enter the first  integer: ");
    scanf("%d",&i);
    printf("Enter the second integer :  ");
    scanf("%d",&j);

    for(i;i<=j;i++)
    {
        if(i%7==2 || i%7==3)
        {
            printf("%d ",i);
        }
    }
    return 0;

}

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/*41. Write a C program to print 3 numbers on a line, starting with 1 and 
printing n lines. Accept the number of lines (n, integer) from the user.
*/

#include <stdio.h>
int main() {

    int a, i;

    // Prompt for user input
    printf("Input number of lines: ");
    scanf("%d", &a);

    // Loop for each line
    for(i = 1; i <= a; i++) {
        // Print i, i squared, and i cubed
        printf("%d %d %d\n", i, i*i, i*i*i);
    }
    
    return 0;
}

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
43. Write a C program that reads two integers p and q, prints p number of lines in a sequence of 1 to b in a line.

#include <stdio.h>
int main() {



    int x, y, i, j, l;

    // Prompt for user input
    printf("Input number of lines: ");
    scanf("%d", &x);
    printf("Number of numbers in a line: ");
    scanf("%d", &y);

    // Loop to generate the pattern
    for(i = 1, l=1; i <= x; i++) {
        for(j = 1; j <= y; j++) {
            printf("%d ", l);		
            l++; 
        }
        printf("\n");
    }

    return 0;
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
48. Write a C program that reads and prints the elements of an array of length 7. Before printing, replace every negative number, zero, with 100.

#include <stdio.h>
int main() {

    int n[5], i, x;
    
    // Input the 5 members of the array
    printf("Input the 5 members of the array:\n");
    for(i = 0; i < 5; i++) {
        scanf("%d", &x);
        if(x > 0) {
            n[i] = x;
        } else {
            n[i] = 100;
        }
    }
    
    // Print the array values
    printf("Array values are: \n");
    for(i = 0; i < 5; i++) {
        printf("n[%d] = %d\n", i, n[i]);
    }
    
    return 0;
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

/* Write a C program to read and print the elements of an array with length 7. 
Before printing, insert the triple of the previous position, starting from the second position.*/

#include <stdio.h>
int main() {

    int n[5], i, x;
    
    // Input the first number of the array
    printf("Input the first number of the array:\n");
    scanf("%d", &x);
    
    // Fill the array with values based on the input
    for(i = 0; i < 5; i++) {
        n[i] = x;
        x = 3 * x;
    }

    // Print the array values
    for(i = 0; i < 5; i++) {
        printf("n[%d] = %d\n", i, n[i]);
    }
    
    return 0;
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
/*Write a C program to read an array of length 5 and
 print the position and value of the array elements of value less than 5.*/

#include <stdio.h>

int main() {

    int arr[5]; // Declare an array of length 5
    int i; // Loop variable

    // Input: Read 5 elements into the array
    printf("Enter 5 integers:\n");
    for (i = 0; i < 5; i++) {
        scanf("%d", &arr[i]); // Read each element
    }

    // Output: Print position and value of elements less than 5
    printf("Elements less than 5:\n");
    for (i = 0; i < 5; i++) {
        if (arr[i] < 5) { // Check if the element is less than 5
            printf("Position: %d, Value: %d\n", i, arr[i]); // Print position and value
        }
    }

    return 0; // Indicate that the program ended successfully
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Write a C program to read an array of length 6, change the first element by the last, the second element by the fifth and the third element by the fourth. Print the elements of the modified array.
#include <stdio.h>

int main() {

    int arr[6]; // Declare an array of length 6
    int i; // Loop variable

    // Input: Read 6 elements into the array
    printf("Enter 6 integers:\n");
    for (i = 0; i < 6; i++) {
        scanf("%d", &arr[i]); // Read each element
    }

    // Modify the array as per the requirements
    arr[0] = arr[5]; // Change the first element to the last
    arr[1] = arr[4]; // Change the second element to the fifth
    arr[2] = arr[3]; // Change the third element to the fourth

    // Output: Print the modified array
    printf("Modified array elements:\n");
    for (i = 0; i < 6; i++) {
        printf("%d ", arr[i]); // Print each element of the modified array
    }
    printf("\n"); // New line for better readability

    return 0; // Indicate that the program ended successfully
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Write a C program to read an array of length 6 and find the smallest element and its position. it also

#include <stdio.h>
int main() {

    int arr[6]; // Declare an array of length 6
    int i; // Loop variable
    int smallest; // Store the smallest element
    int position; // Store the position of the smallest element

    // Input: Read 6 elements into the array
    printf("Enter 6 integers:\n");
    for (i = 0; i < 6; i++) {
        scanf("%d", &arr[i]); // Read each element
    }

    // Initialize smallest and position with the first element
    smallest = arr[0];
    position = 0;

    // Find the smallest element and its position
    for (i = 1; i < 6; i++) {
        if (arr[i] < smallest) { // Check if the current element is smaller
            smallest = arr[i]; // Update the smallest element
            position = i; // Update the position
        }
    }

    // Output: Print the smallest element and its position
    printf("Smallest element: %d\n", smallest);
    printf("Position of the smallest element: %d\n", position);

    return 0; // Indicate that the program ended successfully
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

