# password-check
A simple password checking program in C.
#include <stdio.h>
#include <string.h>

#define MAX_PASSWORD_LENGTH 20

int main() {
    char correctPassword[] = "myPassword123";
    char enteredPassword[MAX_PASSWORD_LENGTH];

    printf("Enter your password: ");
    scanf("%s", enteredPassword);  // This will show the password as you type

    if (strcmp(enteredPassword, correctPassword) == 0) {
        printf("Access granted!\n");
    } else {
        printf("Access denied. Incorrect password.\n");
    }

    return 0;

