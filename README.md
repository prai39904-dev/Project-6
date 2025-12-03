# Project-6
Student Record Management (Name, Roll, Marks)
#include <stdio.h>

struct Student {
    char name[50];
    int roll;
    float marks;
};

int main() {
    int n, i;
    struct Student s[100];

    printf("Enter number of students: ");
    scanf("%d", &n);

    for (i = 0; i < n; i++) {
        printf("Enter name: ");
        scanf("%s", s[i].name);
        printf("Enter roll: ");
        scanf("%d", &s[i].roll);
        printf("Enter marks: ");
        scanf("%f", &s[i].marks);
    }

    printf("\nStudent Records:\n");
    for (i = 0; i < n; i++) {
        printf("Name: %s, Roll: %d, Marks: %.2f\n",
               s[i].name, s[i].roll, s[i].marks);
    }

    return 0;
}
