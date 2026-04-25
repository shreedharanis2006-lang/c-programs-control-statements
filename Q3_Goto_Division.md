## Program 3: Division using goto (Error Handling)

### Code

```c
#include <stdio.h>

int main() {
    int a, b;

start:
    printf("Enter two numbers: ");
    if(scanf("%d %d", &a, &b) != 2) {
        printf("Invalid input! Try again.\n");
        while(getchar() != '\n');
        goto start;
    }

    if(b == 0) {
        printf("Division by zero not allowed! Try again.\n");
        goto start;
    }

    printf("Result = %d\n", a / b);
    return 0;
}
```

### Output

```
Enter two numbers: 10 0
Division by zero not allowed! Try again.
Enter two numbers: 10 2
Result = 5
```
