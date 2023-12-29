© [Aryan Mishra](https://leetcode.com/hola_aryan/)

1929. Concatenation of Array

### C++

```cpp
#include <vector>

class Solution {
public:
    std::vector<int> getConcatenation(std::vector<int>& nums) {
        // Creating a vector with double of its length
        std::vector<int> arr(nums.size() * 2);

        // Running a loop for each element in nums vector
        for (int i = 0; i < nums.size(); i++) {

            arr[i] = nums[i];
            arr[i + nums.size()] = nums[i];
        }

        return arr;
    }
};
```

### Java

```java
class Solution {
    public int[] getConcatenation(int[] nums) {
        // Creating an array with double of its length
        int arr[] = new int[nums.length * 2];

        // Running a loop for each element in nums array
        for (int i = 0; i < nums.length; i++) {

            arr[i] = nums[i];
            arr[i + nums.length] = nums[i];
        }

        return arr;
    }
}
```

### Python

```python
class Solution:
    def getConcatenation(self, nums):
        # Creating a list with double of its length
        arr = [0] * (len(nums) * 2)

        # Running a loop for each element in nums list
        for i in range(len(nums)):
            arr[i] = nums[i]
            arr[i + len(nums)] = nums[i]

        return arr
```

### Python3

```python
class Solution:
    def getConcatenation(self, nums):
        # Creating a list with double of its length
        arr = [0] * (len(nums) * 2)

        # Running a loop for each element in nums list
        for i in range(len(nums)):
            arr[i] = nums[i]
            arr[i + len(nums)] = nums[i]

        return arr
```

### C

```c
#include <stdio.h>
#include <stdlib.h>

int* getConcatenation(int* nums, int numsSize, int* returnSize) {
    // Creating an array with double of its length
    int* arr = (int*)malloc(2 * numsSize * sizeof(int));

    // Running a loop for each element in nums array
    for (int i = 0; i < numsSize; i++) {

        arr[i] = nums[i];
        arr[i + numsSize] = nums[i];
    }

    *returnSize = 2 * numsSize;
    return arr;
}
```

### C#

```csharp
public class Solution {
    public int[] GetConcatenation(int[] nums) {
        // Creating an array with double of its length
        int[] arr = new int[nums.Length * 2];

        // Running a loop for each element in nums array
        for (int i = 0; i < nums.Length; i++) {

            arr[i] = nums[i];
            arr[i + nums.Length] = nums[i];
        }

        return arr;
    }
}
```

### JavaScript

```javascript
class Solution {
    getConcatenation(nums) {
        // Creating an array with double of its length
        const arr = new Array(nums.length * 2);

        // Running a loop for each element in nums array
        for (let i = 0; i < nums.length; i++) {

            arr[i] = nums[i];
            arr[i + nums.length] = nums[i];
        }

        return arr;
    }
}
```

### TypeScript

```typescript
class Solution {
    getConcatenation(nums: number[]): number[] {
        // Creating an array with double of its length
        const arr: number[] = new Array(nums.length * 2);

        // Running a loop for each element in nums array
        for (let i = 0; i < nums.length; i++) {

            arr[i] = nums[i];
            arr[i + nums.length] = nums[i];
        }

        return arr;
    }
}
```