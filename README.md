#include <stdio.h>

int main() {
    int num, sum = 0, digit;

    printf("Enter a number: ");
    scanf("%d", &num);

    // Calculate sum of digits using for loop
    for(int temp = num; temp > 0; temp /= 10) {
        digit = temp % 10;
        sum += digit;
    }

    printf("Sum of digits: %d\n", sum);

    return 0;
}
