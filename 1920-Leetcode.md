© [Aryan Mishra](https://leetcode.com/hola_aryan/)

### C++

```cpp
#include <vector>

class Solution {
public:
    std::vector<int> buildArray(std::vector<int>& nums) {
        // Creating a vector of the same length as the given vector
        std::vector<int> arr(nums.size());

        // Running the loop according to the length
        for (int i = 0; i < nums.size(); i++) {

            // Doing the same thing as explained in logic
            arr[i] = nums[nums[i]];
        }

        return arr;
    }
};
```

### Java

```java
class Solution {
    public int[] buildArray(int[] nums) {
        // Creating an array of the same length as the given array
        int arr[] = new int[nums.length];

        // Running the loop according to the length
        for (int i = 0; i < nums.length; i++) {

            // Doing the same thing as explained in logic
            arr[i] = nums[nums[i]];
        }

        return arr;
    }
}
```

### Python

```python
class Solution:
    def buildArray(self, nums):
        # Creating a list of the same length as the given list
        arr = [0] * len(nums)

        # Running the loop according to the length
        for i in range(len(nums)):

            # Doing the same thing as explained in logic
            arr[i] = nums[nums[i]]

        return arr
```

### Python3

```python
class Solution:
    def buildArray(self, nums):
        # Creating a list of the same length as the given list
        arr = [0] * len(nums)

        # Running the loop according to the length
        for i in range(len(nums)):

            # Doing the same thing as explained in logic
            arr[i] = nums[nums[i]]

        return arr
```

### C

```c
#include <stdio.h>
#include <stdlib.h>

int* buildArray(int* nums, int numsSize, int* returnSize) {
    // Creating an array of the same length as the given array
    int* arr = (int*)malloc(numsSize * sizeof(int));

    // Running the loop according to the length
    for (int i = 0; i < numsSize; i++) {

        // Doing the same thing as explained in logic
        arr[i] = nums[nums[i]];
    }

    *returnSize = numsSize;
    return arr;
}
```

### C#

```csharp
public class Solution {
    public int[] BuildArray(int[] nums) {
        // Creating an array of the same length as the given array
        int[] arr = new int[nums.Length];

        // Running the loop according to the length
        for (int i = 0; i < nums.Length; i++) {

            // Doing the same thing as explained in logic
            arr[i] = nums[nums[i]];
        }

        return arr;
    }
}
```

### JavaScript

```javascript
class Solution {
    buildArray(nums) {
        // Creating an array of the same length as the given array
        const arr = new Array(nums.length);

        // Running the loop according to the length
        for (let i = 0; i < nums.length; i++) {

            // Doing the same thing as explained in logic
            arr[i] = nums[nums[i]];
        }

        return arr;
    }
}
```

### TypeScript

```typescript
class Solution {
    buildArray(nums: number[]): number[] {
        // Creating an array of the same length as the given array
        const arr: number[] = new Array(nums.length);

        // Running the loop according to the length
        for (let i = 0; i < nums.length; i++) {

            // Doing the same thing as explained in logic
            arr[i] = nums[nums[i]];
        }

        return arr;
    }
}
```