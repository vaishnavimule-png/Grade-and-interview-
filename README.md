# Grade-and-interview-
C program 
#include <stdio.h>

int main() {
    char name[50];
    float avg;
    char exp, tech, skill;

    printf("Enter candidate name: ");
    scanf("%[^\n]", name);

    printf("Enter average marks of %s: ", name);
    scanf("%f", &avg);

    printf("Have work experience? (y/n): ");
    scanf(" %c", &exp);

    printf("Have technical knowledge? (y/n): ");
    scanf(" %c", &tech);

    printf("Have skills? (y/n): ");
    scanf(" %c", &skill);

    if (avg > 7 && (exp == 'y' || exp == 'Y' || tech == 'y' || tech == 'Y' || skill == 'y' || skill == 'Y'))
        printf("\n %s has passed the interview!\n", name);
    else
        printf("\n %s has not passed the interview.\n", name);

    return 0;
}
