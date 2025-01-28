# basic-calculator
i made this basic calculator using c language


#include <stdio.h>
int main() {
    char operator;
    int num1, num2, result;
    printf("Enter the first number: ");
    scanf("%d", &num1);
    printf("Enter the second number: ");
    scanf("%d", &num2);
     printf ("Choose an operator +, -, *, / \n");
    scanf(" %c", &operator);
    switch (operator) {
        case '+':
            result = num1 + num2;
            printf("Result: %2d\n", result);
            break;
        case '-':
            result = num1 - num2;
            printf("Result: %2d\n", result);
            break;
        case '*':
            result = num1 * num2;
            printf("Result: %2d\n", result);
            break;
        case '/':
            if (num2 != 0) {
                result = num1 / num2;
                printf("Result: %2d\n", result);
            } else {
                printf("Division by zero is not allowed.\n");
            }
            break;
        default:
            printf("Invalid operator.\n");
    }
    return 0;
}
