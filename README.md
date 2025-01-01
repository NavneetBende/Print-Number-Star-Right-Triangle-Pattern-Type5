PRINTING PATTERN:
10*9*8*7

6*5*4

3*2

1

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows/columns as input from the user and store it in any variable.(‘r‘ in this case).
Run a loop ‘r’ number of times to iterate through each of the rows. From i=0 to i<r The loop should be structured as for( i=0 ; i<r: i++).
Run a nested loop to iterate through the columns. From j=0 to j<r. The loop should be structured as for(j=0 ; j<r; j++).
increment count to calculate the max value.
Run a loop ‘r’ number of times to iterate through each of the rows. From i=0 to i<r The loop should be structured as for( i=0 ; i<r: i++).
Run a nested loop to iterate through the columns. From j=r to j>i. The loop should be structured as for(j=r; j>i; j++).
decrement count and run an if condition if(j!=r).
if true then print star and count else print only count.
outside the nested loop print a newline.
CODE IN C:
#include<stdio.h>
int main()
{
int i,j,r,count; //declaring integer variables i,j for loops , r for number of rows and count for increment in value
count=1; //initialising count
printf("Enter the number of rows :\n"); //Asking user for input
scanf("%d",&r);
for(i=0;i<r;i++)
  { 
    for(j=0;j<=i;j++)
     {
       count+=1;
     }
  } //taking number of rows and saving it in variable r
for(i=0;i<r;i++) // loop for number of rows
  {
    for(j=r;j>i;j--) // loop for digits per each row
      {
        count--;
        if(j!=r) //incrementing count
           printf("*%d",count);
        else
           printf("%d",count); //printing digits
     }
    printf("\n"); // printing newline after each row
  }
}
TAKING INPUT:DISPLAYING OUTPUT:


