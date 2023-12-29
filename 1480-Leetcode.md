© [Aryan Mishra](https://leetcode.com/hola_aryan/)

1480. Running Sum of 1d Array

### C++

```cpp
#include <iostream>
#include <vector>

class Solution {
public:
    // Function to calculate the running sum of an array
    std::vector<int> runningSum(std::vector<int>& nums) {
        // Initializing sum as zero
        int sum = 0;

        // Iterating the array
        for (int i = 0; i < nums.size(); i++) {

            // Finding running sum
            sum += nums[i];

            // Replacing running sum with original element
            nums[i] = sum;
        }

        return nums;
    }
};

int main() {
    Solution solution;
    std::vector<int> nums = {1, 2, 3, 4};
    std::vector<int> result = solution.runningSum(nums);

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
    // Function to calculate the running sum of an array
    public int[] runningSum(int[] nums) {
        // Initializing sum as zero
        int sum = 0;

        // Iterating the array
        for (int i = 0; i < nums.length; i++) {

            // Finding running sum
            sum += nums[i];

            // Replacing running sum with original element
            nums[i] = sum;
        }

        return nums;
    }
}
```

### Python

```python
class Solution:
    # Function to calculate the running sum of an array
    def runningSum(self, nums):
        # Initializing sum as zero
        sum_val = 0

        # Iterating the array
        for i in range(len(nums)):

            # Finding running sum
            sum_val += nums[i]

            # Replacing running sum with original element
            nums[i] = sum_val

        return nums
```

### Python3

```python
class Solution:
    # Function to calculate the running sum of an array
    def runningSum(self, nums):
        # Initializing sum as zero
        sum_val = 0

        # Iterating the array
        for i in range(len(nums)):

            # Finding running sum
            sum_val += nums[i]

            # Replacing running sum with original element
            nums[i] = sum_val

        return nums
```

### C

```c
#include <stdio.h>

// Function to calculate the running sum of an array
int* runningSum(int* nums, int numsSize, int* returnSize) {
    // Initializing sum as zero
    int sum = 0;

    // Iterating the array
    for (int i = 0; i < numsSize; i++) {

        // Finding running sum
        sum += nums[i];

        // Replacing running sum with original element
        nums[i] = sum;
    }

    *returnSize = numsSize;
    return nums;
}

int main() {
    int nums[] = {1, 2, 3, 4};
    int returnSize;

    int* result = runningSum(nums, 4, &returnSize);

    for (int i = 0; i < returnSize; i++) {
        printf("%d ", result[i]);
    }

    printf("\n");

    return 0;
}
```

### C#

```csharp
public class Solution {
    // Function to calculate the running sum of an array
    public int[] RunningSum(int[] nums) {
        // Initializing sum as zero
        int sum = 0;

        // Iterating the array
        for (int i = 0; i < nums.Length; i++) {

            // Finding running sum
            sum += nums[i];

            // Replacing running sum with original element
            nums[i] = sum;
        }

        return nums;
    }
}
```

### JavaScript

```javascript
class Solution {
    // Function to calculate the running sum of an array
    runningSum(nums) {
        // Initializing sum as zero
        let sum = 0;

        // Iterating the array
        for (let i = 0; i < nums.length; i++) {

            // Finding running sum
            sum += nums[i];

            // Replacing running sum with original element
            nums[i] = sum;
        }

        return nums;
    }
}

const solution = new Solution();
console.log(solution.runningSum([1, 2, 3, 4]));
```

### TypeScript

```typescript
class Solution {
    // Function to calculate the running sum of an array
    runningSum(nums: number[]): number[] {
        // Initializing sum as zero
        let sum = 0;

        // Iterating the array
        for (let i = 0; i < nums.length; i++) {

            // Finding running sum
            sum += nums[i];

            // Replacing running sum with original element
            nums[i] = sum;
        }

        return nums;
    }
}

const solution = new Solution();
console.log(solution.runningSum([1, 2, 3, 4]));
```