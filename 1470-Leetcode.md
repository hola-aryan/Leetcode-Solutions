© [Aryan Mishra](https://leetcode.com/hola_aryan/)

1470. Shuffle the Array


Example for understanding this question

Array Elements     = 0,1,2,3  ,  4,5,6,7
Rearrange Elements = 0,4,1,5  ,  2,6,3,7

Pattern for even elements
0-0  2-1  4-2  6-3 (0,1,2,3)

Pattern for Odd elements
1-4  3-5  5-6  7-7 (4,5,6,7)in this case 4 is n

## No need to paste main method while pasting

### C++

```cpp
#include <iostream>
#include <vector>

class Solution {
public:
    // Function to shuffle an array
    std::vector<int> shuffle(std::vector<int>& nums, int n) {
        int cnt = 0;
        // Making an array of the same length
        std::vector<int> arr(2 * n);

        for (int i = 0; i < nums.size(); i++) {
            if (i % 2 == 0) {
                arr[i] = nums[cnt++];
            } else {
                arr[i] = nums[n++];
            }
        }

        return arr;
    }
};

int main() {
    Solution solution;
    std::vector<int> nums = {2, 5, 1, 3, 4, 7};
    int n = 3;
    std::vector<int> result = solution.shuffle(nums, n);

    for (int num : result) {
        std::cout << num << " ";
    }

    std::cout << std::endl;

    return 0;
}
```

### Java

```java
class Solution {
    // Function to shuffle an array
    public int[] shuffle(int[] nums, int n) {
        int cnt = 0;
        // Making an array of the same length
        int[] arr = new int[2 * n];

        for (int i = 0; i < nums.length; i++) {
            if (i % 2 == 0) {
                arr[i] = nums[cnt++];
            } else {
                arr[i] = nums[n++];
            }
        }

        return arr;
    }
}
```

### Python

```python
class Solution:
    # Function to shuffle an array
    def shuffle(self, nums, n):
        cnt = 0
        # Making a list of the same length
        arr = [0] * (2 * n)

        for i in range(len(nums)):
            if i % 2 == 0:
                arr[i] = nums[cnt]
                cnt += 1
            else:
                arr[i] = nums[n]
                n += 1

        return arr
```

### Python3

```python
class Solution:
    # Function to shuffle an array
    def shuffle(self, nums, n):
        cnt = 0
        # Making a list of the same length
        arr = [0] * (2 * n)

        for i in range(len(nums)):
            if i % 2 == 0:
                arr[i] = nums[cnt]
                cnt += 1
            else:
                arr[i] = nums[n]
                n += 1

        return arr
```

### C

```c
#include <stdio.h>
#include <stdlib.h>

// Function to shuffle an array
int* shuffle(int* nums, int numsSize, int n, int* returnSize) {
    int cnt = 0;
    // Making an array of the same length
    int* arr = (int*)malloc(2 * n * sizeof(int));

    for (int i = 0; i < numsSize; i++) {
        if (i % 2 == 0) {
            arr[i] = nums[cnt++];
        } else {
            arr[i] = nums[n++];
        }
    }

    *returnSize = numsSize;
    return arr;
}

int main() {
    int nums[] = {2, 5, 1, 3, 4, 7};
    int n = 3;
    int returnSize;

    int* result = shuffle(nums, 6, n, &returnSize);

    for (int i = 0; i < returnSize; i++) {
        printf("%d ", result[i]);
    }

    printf("\n");

    free(result);

    return 0;
}
```

### C#

```csharp
public class Solution {
    // Function to shuffle an array
    public int[] Shuffle(int[] nums, int n) {
        int cnt = 0;
        // Making an array of the same length
        int[] arr = new int[2 * n];

        for (int i = 0; i < nums.Length; i++) {
            if (i % 2 == 0) {
                arr[i] = nums[cnt++];
            } else {
                arr[i] = nums[n++];
            }
        }

        return arr;
    }
}
```

### JavaScript

```javascript
class Solution {
    // Function to shuffle an array
    shuffle(nums, n) {
        let cnt = 0;
        // Making an array of the same length
        const arr = new Array(2 * n);

        for (let i = 0; i < nums.length; i++) {
            if (i % 2 === 0) {
                arr[i] = nums[cnt++];
            } else {
                arr[i] = nums[n++];
            }
        }

        return arr;
    }
}

const solution = new Solution();
console.log(solution.shuffle([2, 5, 1, 3, 4, 7], 3));
```

### TypeScript

```typescript
class Solution {
    // Function to shuffle an array
    shuffle(nums: number[], n: number): number[] {
        let cnt = 0;
        // Making an array of the same length
        const arr: number[] = new Array(2 * n);

        for (let i = 0; i < nums.length; i++) {
            if (i % 2 === 0) {
                arr[i] = nums[cnt++];
            } else {
                arr[i] = nums[n++];
            }
        }

        return arr;
    }
}

const solution = new Solution();
console.log(solution.shuffle([2, 5, 1, 3, 4, 7], 3));
```