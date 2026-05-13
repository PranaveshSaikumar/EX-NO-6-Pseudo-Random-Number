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
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    int n, min, max, i, num;

    srand(time(0));

    printf("Enter how many random numbers: ");
    scanf("%d", &n);

    printf("Enter minimum value: ");
    scanf("%d", &min);

    printf("Enter maximum value: ");
    scanf("%d", &max);

    printf("Random numbers are:\n");

    for(i = 0; i < n; i++) {
        num = (rand() % (max - min + 1)) + min;
        printf("%d\n", num);
    }

    return 0;
}
```

# OUTPUT:
<img width="1345" height="826" alt="image" src="https://github.com/user-attachments/assets/85b5fdb1-ea59-4df6-bcde-5d40099eb9a5" />


# RESULT:
Thus the implementation of Pseudorandom Number Generation had been executed successfully.
