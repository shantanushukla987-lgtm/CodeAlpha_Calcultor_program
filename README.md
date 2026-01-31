#include <stdio.h>

int main() {
    int choice;
    float a, b, result;

    printf("Enter two numbers: ");
    scanf("%f %f", &a, &b);

    printf("\nChoose Operation:\n");
    printf("1. Addition\n");
    printf("2. Subtraction\n");
    printf("3. Multiplication\n");
    printf("4. Division\n");
    printf("Enter choice: ");
    scanf("%d", &choice);

    switch (choice) {
        case 1:
            result = a + b;
            printf("Addition = %.2f", result);
            break;

        case 2:
            result = a - b;
            printf("Subtraction = %.2f", result);
            break;

        case 3:
            result = a * b;
            printf("Multiplication = %.2f", result);
            break;

        case 4:
            if (b != 0)
                printf("Division = %.2f", a / b);
            else
                printf("Error! Division by zero.");
            break;

        default:
            printf("Invalid choice!");
    }
    return 0;
}
