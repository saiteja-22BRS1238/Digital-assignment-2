#include <stdio.h>

void divide(int arr[], int size);

int main() {
    int size, i;
    printf("Enter the size of the array: ");
    scanf("%d", &size);

    int arr[size];

    printf("Enter %d elements of the array:\n", size);
    for (i = 0; i < size; i++) {
        scanf("%d", &arr[i]);
    }

    divide(arr, size);

    return 0;
}

void divide(int arr[], int size) {
    if (size == 1) {
        printf("Array is divided into individual elements\n");
        return;
    }

    int mid = size / 2;
    int left[mid], right[size - mid];
    int i;

    for (i = 0; i < mid; i++) {
        left[i] = arr[i];
    }

    for (i = mid; i < size; i++) {
        right[i - mid] = arr[i];
    }

    printf("Left Half: ");
    for (i = 0; i < mid; i++) {
        printf("%d ", left[i]);
    }
    printf("\n");

    printf("Right Half: ");
    for (i = 0; i < size - mid; i++) {
        printf("%d ", right[i]);
    }
    printf("\n");

    divide(left, mid);
    divide(right, size - mid);
}
