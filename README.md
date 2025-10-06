# Convert--Integer-to-binary-
To convert integer to binary 
#include <stdio.h>

int main() {
    int num, binary[32], i = 0;

    printf("Enter an integer value: ");
    scanf("%d", &num);

    
    if (num == 0) {
        printf("Binary value: 0\n");
        return 0;
    }

    
    while (num > 0) {
        binary[i] = num % 2;   // store remainder (0 or 1)
        num = num / 2;         // divide number by 2
        i++;
    }

    
  
    printf("Binary value: ");
    for (int j = i - 1; j >= 0; j--) {
        printf("%d", binary[j]);
    }

    printf("\n");
    return 0;
}
