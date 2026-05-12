# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.

Seed the random number generator using the current time(i.e) rand(time(0));

Get the number of randon number to generate.


Pass the value for number of iterations and print the numbers.

End the program.
 
# PROGRAM:
~~~
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int n, i, rn;

    srand(time(0));

    printf("Enter the number of random number: ");
    scanf("%d", &n);

    printf("Generated random number are:\n");

    for(i = 0; i < n; i++)
    {
        rn = rand() % 9000 + 1000;   
        printf("%d\n",rn );
    }

    return 0;
}
~~~
# OUTPUT:
<img width="1305" height="586" alt="ex6" src="https://github.com/user-attachments/assets/132da4eb-f02e-4ce4-9bf5-5d07ffff9006" />

# RESULT:
Thus, the pseudorandom numbers were generated successfully using the standard library function.
