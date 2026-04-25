## Program 4: Number Guessing Game

### Code

```c
#include <stdio.h>

int main() {
    int guess, number = 7;

    while(1) {
        printf("Enter your guess (-1 to exit): ");
        scanf("%d", &guess);

        if(guess == -1) {
            return 0;
        }

        if(guess == number) {
            printf("Correct guess!\n");
            break;
        } else {
            printf("Wrong guess. Try again.\n");
        }
    }

    return 0;
}
```

### Output

```
Enter your guess: 3
Wrong guess. Try again.
Enter your guess: 7
Correct guess!
```
