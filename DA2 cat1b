#include <stdio.h>
#include <stdlib.h>
#include <string.h>
typedef struct Employee {
    char name[50];
    int age;
    char position[50];
    char dateOfJoining[11]; 
} Employee;
int cmpName(const void* a, const void* b) {
    Employee* empA = (Employee*)a;
    Employee* empB = (Employee*)b;
    return strcmp(empA->name, empB->name);
}
int cmpJoinDate(const void* a, const void* b) {
    Employee* empA = (Employee*)a;
    Employee* empB = (Employee*)b;
   
    int dayA, monthA, yearA, dayB, monthB, yearB;
    sscanf(empA->dateOfJoining, "%d/%d/%d", &dayA, &monthA, &yearA);
    sscanf(empB->dateOfJoining, "%d/%d/%d", &dayB, &monthB, &yearB);
    if (yearA != yearB) {
        return yearA - yearB;
    } else if (monthA != monthB) {
        return monthA - monthB;
    } else {
        return dayA - dayB;
    }
}
int main() {
    int n;
    printf("Enter the number of employees: ");
    scanf("%d", &n);
    Employee employees[n];
    for (int i = 0; i < n; i++) {
        printf("Enter details of employee %d:\n", i+1);
        printf("Name: ");
        scanf("%s", employees[i].name);
        printf("Age: ");
        scanf("%d", &employees[i].age);
        printf("Position: ");
        scanf("%s", employees[i].position);
        printf("Date of joining (dd/mm/yyyy): ");
        scanf("%s", employees[i].dateOfJoining);
    }
    qsort(employees, n, sizeof(Employee), cmpName);

    printf("\nEmployee List sorted by name:\n\n");
    for (int i = 0; i < n; i++) {
        printf("Name: %s\n", employees[i].name);
        printf("Age: %d\n", employees[i].age);
        printf("Position: %s\n", employees[i].position);
        printf("Date of Joining: %s\n\n", employees[i].dateOfJoining);
    }
    qsort(employees, n, sizeof(Employee), cmpJoinDate);

    printf("\nEmployee List sorted by date of joining:\n\n");
    for (int i = 0; i < n; i++) {
        printf("Name: %s\n", employees[i].name);
        printf("Age: %d\n", employees[i].age);
        printf("Position: %s\n", employees[i].position);
        printf("Date of Joining: %s\n\n", employees[i].dateOfJoining);
    }

    return 0;
}
