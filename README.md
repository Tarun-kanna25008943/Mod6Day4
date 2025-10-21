# EX-04 Program to Calculate Student’s Age at the Time of Admission Using Nested Structures and Pointer

## AIM:
To write a C program that calculates the age of a student at the time of admission using nested structures and a structure pointer.
The program should read the student’s registration number, name, birth date, and admission date as input.

## ALGORITHM:

1. Start
2. Define a structure admission with members:
    * rego → registration number
    * ch[100] → student name
    * date1, month1, year1 → date of birth
    * date, month, year → admission date
3. Declare a structure variable b.
4. Read the following inputs using scanf():
    * Registration number
    * Student name
    * Birth date (day, month, year)
    * Admission date (day, month, year)
5. Calculate approximate age:
    * age = b.year - b.year1
6. Print the calculated age as the student’s approximate age at the time of admission.
7. Stop

## PROGRAM:
```
#include <stdio.h>

struct admission
{
    int rego;
    char ch[100];
    int date1,month1,year1;
    int date,month,year;
};

int main()
{
    struct admission b;
    printf("Enter the reg no: ");
    scanf("%d",&b.rego);
    printf("\nEnter the name: ");
    scanf("%s",b.ch);
    printf("\nEnter your DOB: ");
    scanf("%d %d %d",&b.date1,&b.month1,&b.year1);
    printf("\nEnter the current date: ");
    scanf("%d %d %d",&b.date,&b.month,&b.year);
    
    int age = b.year - b.year1;
    
    printf("\nApproximate Age of Student at the Time of Admission\n%d Years",age);
}
```
## OUTPUT:
<img width="671" height="321" alt="image" src="https://github.com/user-attachments/assets/e56e7fce-fa51-40c5-83f4-482d3bdac975" />

## RESULT:
The program successfully reads student details using nested structures and a structure pointer, and calculates the student’s age at the time of admission.
