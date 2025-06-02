# EX 34 C program to read a file name from user and create that file and insert student roll numbers in to that file.
## DATE: 12/04/2025
## AIM:
To write a C program to read a file name from user and create that file and insert student roll numbers in to that file.

## Algorithm
1.Start the program and declare a file pointer and a character array for the file name.

2.Read the file name from the user and open it in write mode using fopen().

3.Read the number of student roll numbers and their values from the user.

4.Write each roll number into the file using fprintf().

5.Close the file and display a success message.

## Program:
```
/*
C program to read a file name from user and create that file and insert student roll numbers in to that file.
Developed by: RUPESH J
RegisterNumber:  212222060204
*/
#include <stdio.h>

int main()
{
    char filename[100];
    FILE *fp;
    int n, i, roll;

    printf("Enter the file name to create: ");
    scanf("%s", filename);

    fp = fopen(filename, "w");

    if(fp == NULL)
    {
        printf("File creation failed.\n");
        return 1;
    }

    printf("Enter the number of student roll numbers: ");
    scanf("%d", &n);

    printf("Enter the roll numbers:\n");
    for(i = 0; i < n; i++)
    {
        scanf("%d", &roll);
        fprintf(fp, "%d\n", roll);
    }

    fclose(fp);
    printf("Roll numbers written to file '%s' successfully.\n", filename);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/dc86fd37-92be-427b-9c60-9c67b85aeb4d)


## Result:
Thus the program was executed and the output was verified successfully.
