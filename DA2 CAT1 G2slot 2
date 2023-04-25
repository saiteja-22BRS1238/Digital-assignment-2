#include <stdio.h>


int sumOfDigits(int n) {
    int sum = 0;
    while (n > 0) {
        sum += n % 10;
        n /= 10;
    }
    return sum;
}

int main() {
    int sum = 0;
    
    
    for (int i = 1000; i <= 9998; i += 2) {
        sum += i;
    }
    
    
    while (sum > 9) {
        sum = sumOfDigits(sum);
    }
  
    if (sum % 2 == 0) {
        printf("Even found\n");
    } else {
        printf("Odd found\n");
    }
    
    return 0;
}
