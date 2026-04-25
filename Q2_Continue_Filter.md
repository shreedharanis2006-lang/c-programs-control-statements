# c-programs-control-statements
## Program 2: Print 1–100 (Skip multiples of 3 and numbers with digit 5)

### Code

```c
#include <stdio.h>

int containsFive(int num) {
    while(num > 0) {
        if(num % 10 == 5)
            return 1;
        num /= 10;
    }
    return 0;
}

int main() {
    for(int i = 1; i <= 100; i++) {
        if(i % 3 == 0 || containsFive(i)) {
            continue;
        }
        printf("%d ", i);
    }
    return 0;
}
```

### Output (partial)

```
1 2 4 7 8 11 13 14 ...
```
