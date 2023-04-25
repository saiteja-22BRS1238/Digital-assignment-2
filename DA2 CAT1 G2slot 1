#include <stdio.h>

int main() {
    float chennai_temps[7];
    float delhi_temps[7];
    float haveri_temps[7];
    float gangtok_temps[7];

    
    printf("Enter the temperature of Chennai for each day of the week (in degrees Celsius):\n");
    for (int i = 0; i < 7; i++) {
        scanf("%f", &chennai_temps[i]);

      
        if (chennai_temps[i] < 28 || chennai_temps[i] > 33) {
            printf("Invalid temperature! Temperature should be between 28C and 33C.\n");
            return 0;
        }
    }

    
    for (int i = 0; i < 7; i++) {
        delhi_temps[i] = chennai_temps[i] - 8;
        haveri_temps[i] = chennai_temps[i] + 5;
    }

    for (int i = 0; i < 7; i++) {
        gangtok_temps[i] = haveri_temps[i] - delhi_temps[i];
    }

    
    printf("The temperature of Gangtok for each day of the week (in degrees Celsius):\n");
    for (int i = 0; i < 7; i++) {
        printf("%.2f\n", gangtok_temps[i]);
    }

    return 0;
}
