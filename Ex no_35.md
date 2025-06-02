# EX 35 C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.
## DATE: 12/04/2025
## AIM:
To write a C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.

## Algorithm
1.Start the program and declare a file pointer.

2.Use fopen() in write mode to create and open the file "Hospital.txt".

3.Check if the file was created and opened successfully and display a message.

4.Close the file using fclose() after confirming successful opening.

5.Display a message indicating the file was closed successfully. 

## Program:
```
/*
C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.
Developed by: RUPESH J
RegisterNumber:  212222060204
*/
#include <stdio.h>

int main()
{
    FILE *fp;

    fp = fopen("Hospital.txt", "w");

    if(fp == NULL)
    {
        printf("File creation or opening failed.\n");
        return 1;
    }

    printf("File 'Hospital.txt' created and opened successfully.\n");

    fclose(fp);

    printf("File 'Hospital.txt' closed successfully.\n");

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/203da4b4-ba2b-4776-9804-8bf72ffe9524)


## Result:
Thus the program was executed and the output was verified successfully.
