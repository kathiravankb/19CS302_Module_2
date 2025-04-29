# EX 9 C program to find the sum of odd digits using do while loop.
## DATE: 29/04/2025
## AIM:
To write a C program to find the sum of odd digits using do while loop.

## Algorithm
1.Start
2.Declare num, digit, and sum = 0.
3.Input the number num.
4.Use a do-while loop:
5.Get the last digit using digit = num % 10.
6.If digit is odd (digit % 2 != 0), add it to sum.
7.Remove the last digit: num = num / 10.
8.Repeat until num > 0.
9.Print the sum.
10.End   

## Program:
```
#include <stdio.h>

int main() {
    int num, digit, sum = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    int temp = num; // Store original number for display

    do {
        digit = num % 10;
        if (digit % 2 != 0) {
            sum += digit;
        }
        num = num / 10;
    } while (num > 0);

    printf("Sum of odd digits in %d is: %d\n", temp, sum);

    return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/dcdb906e-0e3e-452b-862e-7c19f823b51e)


## Result:
Thus the program was executed and the output was verified successfully.
