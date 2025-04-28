# EX 9 C program to find the sum of odd digits using do while loop.
## DATE: 25/04/2025
## AIM:
To write a C program to find the sum of odd digits using do while loop.

## Algorithm
Start.

Declare variables: number, digit, sum.

Initialize sum = 0.

Input the number.

Use a do-while loop:

Find the last digit (digit = number % 10).

If the digit is odd (digit % 2 != 0):

Add it to sum.

Remove the last digit (number = number / 10).

Repeat the loop until number > 0.

Print the value of sum.

End.

## Program:
```
#include <stdio.h>

int main() {
    int number, digit, sum = 0;

    printf("Enter a number: ");
    scanf("%d", &number);

    if (number == 0) {
        printf("Sum of odd digits: 0\n");
        return 0;
    }

    if (number < 0) {
        number = -number; // Make number positive if negative
    }

    do {
        digit = number % 10;
        if (digit % 2 != 0) {
            sum += digit;
        }
        number = number / 10;
    } while (number > 0);

    printf("Sum of odd digits: %d\n", sum);

    return 0;
}

```

## Output:

![ChatGPT Image Apr 28, 2025, 05_53_40 PM](https://github.com/user-attachments/assets/7874ed56-f45d-4f92-a257-513a0d1bdfe7)


## Result:
Thus the program was executed and the output was verified successfully.
