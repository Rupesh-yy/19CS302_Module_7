# EX 31 C program to find the smallest among three numbers using Structure.
## DATE: 12/04/2025
## AIM:
To write a C program to find the smallest among three numbers using Structure.

## Algorithm
1.Start the program and define a structure with three integer fields.

2.Declare a structure variable to store the three numbers.

3.Read the values of the three numbers from the user.

4.Compare the three numbers to find the smallest.

5.Display the smallest number and end the program. 

## Program:
```
/*
C program to find the smallest among three numbers using Structure.
Developed by: RUPESH J
RegisterNumber:  212222060204
*/
#include <stdio.h>

struct Numbers
{
    int num1, num2, num3;
};

int main()
{
    struct Numbers n;

    printf("Enter three numbers: ");
    scanf("%d %d %d", &n.num1, &n.num2, &n.num3);

    int smallest = n.num1;

    if(n.num2 < smallest)
    {
        smallest = n.num2;
    }

    if(n.num3 < smallest)
    {
        smallest = n.num3;
    }

    printf("The smallest number is: %d\n", smallest);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/d887c1cc-83cb-4eee-aa33-50eed14d157c)


## Result:
Thus the program was executed and the output was verified successfully.
