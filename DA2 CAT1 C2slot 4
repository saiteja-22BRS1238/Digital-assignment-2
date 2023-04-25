#include <stdio.h>

int main() {
    char type_of_car[10];
    float price_of_car, extra_fitting_price, total, discount, gst, net;

    printf("Enter type of car: ");
    scanf("%s", type_of_car);

    printf("Enter price of car: ");
    scanf("%f", &price_of_car);

    printf("Enter extra fitting price: ");
    scanf("%f", &extra_fitting_price);

    // Calculate total price
    total = price_of_car + extra_fitting_price;

    // Calculate discount and GST based on car type
    if (strcmp(type_of_car, "Hatchback") == 0) {
        discount = total * 0.03;
        gst = (total - discount) * 0.12;
    } else if (strcmp(type_of_car, "Sedan") == 0) {
        discount = total * 0.05;
        gst = (total - discount) * 0.12;
    } else if (strcmp(type_of_car, "SUV") == 0) {
        discount = total * 0.10;
        gst = (total - discount) * 0.12;
    } else if (strcmp(type_of_car, "MUV") == 0) {
        discount = total * 0.15;
        gst = (total - discount) * 0.12;
    } else {
        printf("Invalid type of car\n");
        return 0;
    }
    net = total - discount + gst;

    printf("Net amount to be paid: %.2f\n", net);

    return 0;
}
