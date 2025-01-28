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
![image](https://github.com/user-attachments/assets/8ad23f72-8228-4545-8728-12e767dc1251)
![image](https://github.com/user-attachments/assets/f176a944-aef8-436c-8e0b-8ac619316533)

