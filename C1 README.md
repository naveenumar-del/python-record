EX-01-Datatypes-Operators
AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

ALGORITHM:
Declare three character variables to store the input characters.
Use the scanf function to read the characters one by one from the user.
Print the characters in reverse order using the printf function.
End the program.
PROGRAM:
#include <stdio.h>

int main() {
    char a, b, c;

    printf("Enter first character: ");
    scanf(" %c", &a);

    printf("Enter second character: ");
    scanf(" %c", &b);

    printf("Enter third character: ");
    scanf(" %c", &c);

    printf("Characters in reverse order: %c %c %c\n", c, b, a);

    return 0;
}

OUTPUT:
<img width="1920" height="1139" alt="Screenshot 2025-12-23 202119" src="https://github.com/user-attachments/assets/0727e62a-2e1e-4735-a1ec-7fed1a31d301" />


RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.

EX-02- Conditional-Statements
AIM:
Write a C program to read A values and check whether A is positive number or not.

ALGORITHM:
Declare a variable to store the input value A.
Use the scanf function to read the value of A from the user.
Check if the value of A is greater than zero.
If A is greater than zero, print a message indicating that it's a positive number.
Otherwise, print a message indicating that it's not a positive number. 6.End the program.
PROGRAM:
#include <stdio.h>

int main() {
    int A;

    printf("Enter a number: ");
    scanf("%d", &A);

    if (A > 0)
        printf("%d is a positive number.\n", A);
    else
        printf("%d is not a positive number.\n", A);

    return 0;
}

OUTPUT:
<img width="1920" height="1142" alt="image" src="https://github.com/user-attachments/assets/a7e3fbab-3a0b-4078-b22f-3eb4239df623" />


RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.

EX-03- Operators-Expressions
AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

ALGORITHM:
Declare variables to store the two fraction numbers and the result.
Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
Use the scanf function to read the numerator and denominator of the first fraction.
Repeat steps 2 and 3 to get the second fraction from the user.
Calculate the decimal values of both fractions by dividing the numerators by the denominators.
Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
Print the minimum value.
PROGRAM:
#include <stdio.h>

int main() {
    float a, b, min;

    printf("Enter first number: ");
    scanf("%f", &a);

    printf("Enter second number: ");
    scanf("%f", &b);

    min = (a < b) ? a : b;

    printf("Minimum number is: %.2f\n", min);

    return 0;
}

OUTPUT:
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/de3c4f6c-13c6-43ec-96b2-59fbf43ed57c" />


RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.

EX-04- Using Conditional Statements
AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

ALGORITHM:
Declare a variable to store the input value.
Use the scanf function to read the input value from the user.
Use an if statement to check if the input value is equal to 1.
If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
Otherwise, print a message indicating that it's not equal to 1.
End the program.
PROGRAM:
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num == 1)
        printf("The number is equal to 1.\n");

    return 0;
}

OUTPUT:
<img width="1920" height="1142" alt="image" src="https://github.com/user-attachments/assets/586b2286-26ed-476a-9edb-4d9d56654a94" />


RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully

EX-05- Calculating Total, Percentage, And Division Using Conditional Statements
AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.

ALGORITHM:
Start
Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
Input the marks for three subjects.
Calculate total marks: tot = m1 + m2 + m3
Calculate percentage: per = tot / 3
Display total and percentage.
Check if all marks are greater than or equal to 40:
If yes: a. If percentage >= 60: Print “Division = First” b. Else if percentage >= 48: Print “Division = Second” c. Else if percentage >= 36: Print “Division = Pass”
Else: Print “Division = Fail”
End
PROGRAM:
#include <stdio.h>

int main() {
    float m1, m2, m3, total, percentage;

    printf("Enter marks of three subjects: ");
    scanf("%f %f %f", &m1, &m2, &m3);


    total = m1 + m2 + m3;
    percentage = (total / 300) * 100; // assuming each subject is out of 100

    printf("\nTotal Marks = %.2f", total);
    printf("\nPercentage = %.2f%%", percentage);


    if (m1 < 35 || m2 < 35 || m3 < 35) {
        printf("\nResult: Fail (Less than 35 marks in one or more subjects)\n");
    }
    else {
        if (percentage >= 60)
            printf("\nResult: First Division\n");
        else if (percentage >= 45)
            printf("\nResult: Second Division\n");
        else if (percentage >= 35)
            printf("\nResult: Pass Division\n");
        else
            printf("\nResult: Fail\n");
    }

    return 0;
}

OUTPUT:
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/cfe71910-b432-4090-b639-84b0efae6958" />


RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.
