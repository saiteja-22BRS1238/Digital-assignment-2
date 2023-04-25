#include <stdio.h>

int power(int x, int n);

int main() {
    int x, n, result;
    printf("Enter a number: ");
    scanf("%d", &x);
    printf("Enter the power (<= 5): ");
    scanf("%d", &n);
    if(n > 5) {
        printf("Error: Power should be less than or equal to 5.");
        return 0;
    }
    result = power(x, n);
    printf("%d raised to the power %d is %d\n", x, n, result);
    return 0;
}

int power(int x, int n) {
    if(n == 0) {
        return 1;
    } else {
        return x * power(x, n-1);
    }
}
