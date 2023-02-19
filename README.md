#include <stdio.h>
#include <string.h>

int main() {
    char phone_number[11], *p;
    int i, len;

    printf("Enter a 10-digit phone number: ");
    scanf("%s", phone_number);

    len = strlen(phone_number);
    p = phone_number + len - 1; // point to the last character

    printf("Reversed phone number: ");
    for (i = 0; i < len; i++) {
        printf("%c", *p);
        p--;
    }

    printf("\n");
    return 0;
}
