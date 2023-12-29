© [Aryan Mishra](https://leetcode.com/hola_aryan/)

1672. Richest Customer Wealth

### C++

```cpp
#include <iostream>
#include <vector>

class Solution {
public:
    // Function to find the maximum wealth among the customers
    int maximumWealth(std::vector<std::vector<int>>& accounts) {
        // Taking the minimum value as max
        int max = INT_MIN;

        // Iterating each row (person)
        for (int i = 0; i < accounts.size(); i++) {
            int sum = 0;
            // Iterating each column to calculate total wealth they have
            for (int j = 0; j < accounts[i].size(); j++) {
                sum += accounts[i][j];
            }

            // Checking if the current sum is greater than the previous max 
            if (sum > max) {
                max = sum;
            }
        }

        return max;
    }
};

int main() {
    Solution solution;
    std::vector<std::vector<int>> accounts = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
    std::cout << solution.maximumWealth(accounts) << std::endl;
    return 0;
}
```

### Java

```java
class Solution {
    // Function to find the maximum wealth among the customers
    public int maximumWealth(int[][] accounts) {
        // Taking the minimum value as max
        int max = Integer.MIN_VALUE;

        // Iterating each row (person)
        for (int i = 0; i < accounts.length; i++) {
            int sum = 0;
            // Iterating each column to calculate total wealth they have
            for (int j = 0; j < accounts[i].length; j++) {
                sum += accounts[i][j];
            }

            // Checking if the current sum is greater than the previous max 
            if (sum > max) {
                max = sum;
            }
        }

        return max;
    }
}
```

### Python

```python
class Solution:
    # Function to find the maximum wealth among the customers
    def maximumWealth(self, accounts):
        # Taking the minimum value as max
        max_wealth = float('-inf')

        # Iterating each row (person)
        for i in range(len(accounts)):
            wealth = sum(accounts[i])
            
            # Checking if the current wealth is greater than the previous max
            if wealth > max_wealth:
                max_wealth = wealth
        
        return max_wealth
```

### Python3

```python
class Solution:
    # Function to find the maximum wealth among the customers
    def maximumWealth(self, accounts):
        # Taking the minimum value as max
        max_wealth = float('-inf')

        # Iterating each row (person)
        for i in range(len(accounts)):
            wealth = sum(accounts[i])
            
            # Checking if the current wealth is greater than the previous max
            if wealth > max_wealth:
                max_wealth = wealth
        
        return max_wealth
```

### C

```c
#include <stdio.h>
#include <limits.h>

// Function to find the maximum wealth among the customers
int maximumWealth(int accounts[][3], int rows, int cols) {
    // Taking the minimum value as max
    int max = INT_MIN;

    // Iterating each row (person)
    for (int i = 0; i < rows; i++) {
        int sum = 0;
        // Iterating each column to calculate total wealth they have
        for (int j = 0; j < cols; j++) {
            sum += accounts[i][j];
        }

        // Checking if the current sum is greater than the previous max 
        if (sum > max) {
            max = sum;
        }
    }

    return max;
}

int main() {
    int accounts[][3] = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
    printf("%d\n", maximumWealth(accounts, 3, 3));
    return 0;
}
```

### C#

```csharp
public class Solution {
    // Function to find the maximum wealth among the customers
    public int MaximumWealth(int[][] accounts) {
        // Taking the minimum value as max
        int max = int.MinValue;

        // Iterating each row (person)
        for (int i = 0; i < accounts.Length; i++) {
            int sum = 0;
            // Iterating each column to calculate total wealth they have
            for (int j = 0; j < accounts[i].Length; j++) {
                sum += accounts[i][j];
            }

            // Checking if the current sum is greater than the previous max 
            if (sum > max) {
                max = sum;
            }
        }

        return max;
    }
}
```

### JavaScript

```javascript
class Solution {
    // Function to find the maximum wealth among the customers
    maximumWealth(accounts) {
        // Taking the minimum value as max
        let max = Number.MIN_SAFE_INTEGER;

        // Iterating each row (person)
        for (let i = 0; i < accounts.length; i++) {
            let sum = 0;
            // Iterating each column to calculate total wealth they have
            for (let j = 0; j < accounts[i].length; j++) {
                sum += accounts[i][j];
            }

            // Checking if the current sum is greater than the previous max 
            if (sum > max) {
                max = sum;
            }
        }

        return max;
    }
}

const solution = new Solution();
console.log(solution.maximumWealth([[1, 2, 3], [4, 5, 6], [7, 8, 9]]));
```

### TypeScript

```typescript
class Solution {
    // Function to find the maximum wealth among the customers
    maximumWealth(accounts: number[][]): number {
        // Taking the minimum value as max
        let max = Number.MIN_SAFE_INTEGER;

        // Iterating each row (person)
        for (let i = 0; i < accounts.length; i++) {
            let sum = 0;
            // Iterating each column to calculate total wealth they have
            for (let j = 0; j < accounts[i].length; j++) {
                sum += accounts[i][j];
            }

            // Checking if the current sum is greater than the previous max 
            if (sum > max) {
                max = sum;
            }
        }

        return max;
    }
}

const solution = new Solution();
console.log(solution.maximumWealth([[1, 2, 3], [4, 5, 6], [7, 8, 9]]));
```