## Program 5: Array Control Flow Behavior

### Code

```c
#include <stdio.h>

int main() {
    int arr[] = {10, -5, 20, 0, 150, 30};

    for(int i = 0; i < 6; i++) {
        if(arr[i] < 0) {
            continue;
        }

        if(arr[i] == 0) {
            break;
        }

        if(arr[i] > 100) {
            return 0;
        }

        printf("%d ", arr[i]);
    }

    return 0;
}
```

### Output

```
10 20
```
