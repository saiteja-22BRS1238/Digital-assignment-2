#include <stdio.h>
#include <ctype.h>

#define MAX_LEN 100

int main() {
    char str[MAX_LEN];
    int counts[5] = {0}; 
    int i = 0;

    printf("Enter a string: ");
    fgets(str, MAX_LEN, stdin);

    while (str[i] != '\0') {
        if (isupper(str[i])) {
            counts[0]++;
            printf("%c is an uppercase alphabet\n", str[i]);
        } else if (islower(str[i])) {
            counts[1]++;
            printf("%c is a lowercase alphabet\n", str[i]);
        } else if (isdigit(str[i])) {
            counts[2]++;
            printf("%c is a digit\n", str[i]);
        } else if (isspace(str[i])) {
            counts[3]++;
            printf("%c is a whitespace character\n", str[i]);
        } else {
            counts[4]++;
            printf("%c is a special symbol\n", str[i]);
        }
        i++;
    }

    printf("\nCounts:\n");
    printf("Uppercase alphabets: %d\n", counts[0]);
    printf("Lowercase alphabets: %d\n", counts[1]);
    printf("Digits: %d\n", counts[2]);
    printf("Whitespace characters: %d\n", counts[3]);
    printf("Special symbols: %d\n", counts[4]);

    return 0;
}
