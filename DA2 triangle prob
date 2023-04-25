#include <stdio.h>

int main() {
    int acute_count = 0, right_count = 0, obtuse_count = 0, wrong_count = 0;

    for (int i = 0; i < 5; i++) {
        int angle1, angle2, angle3;
        printf("Enter angle 1: ");
        scanf("%d", &angle1);
        printf("Enter angle 2: ");
        scanf("%d", &angle2);
        printf("Enter angle 3: ");
        scanf("%d", &angle3);

        if (angle1 + angle2 + angle3 != 180) {
            printf("Wrong entry, try again\n");
            wrong_count++;
            i--;
        }
        else {
            if (angle1 < 90 && angle2 < 90 && angle3 < 90)
                acute_count++;
            else if (angle1 == 90 || angle2 == 90 || angle3 == 90)
                right_count++;
            else
                obtuse_count++;
        }
    }

    printf("Acute Angled Triangle: %d\n", acute_count);
    printf("Right Angled Triangle: %d\n", right_count);
    printf("Obtuse Angled Triangle: %d\n", obtuse_count);
    printf("Wrong Entries: %d\n", wrong_count);

    return 0;
}
