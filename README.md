![Capture](https://user-images.githubusercontent.com/124594384/219952848-005a80f2-da1d-43f3-8539-39babb7edd47.PNG)
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


In this program, we first declare a character array to hold the phone number and a pointer p to point to its last character. We then prompt the user to enter a 10-digit phone number, and read it into the array using scanf.

Next, we determine the length of the phone number using strlen, and set p to point to the last character in the array. We then use a loop to print the phone number in reverse order by iterating through the array using the pointer p, and printing each character using the printf function.

Finally, we print a newline character and return 0 to indicate successful program execution.
