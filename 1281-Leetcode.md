© [Aryan Mishra](https://leetcode.com/hola_aryan/)

1281. Subtract the Product and Sum of Digits of an Integer

### C++

```cpp
#include <iostream>

class Solution {
public:
    // Function to subtract the product and sum of digits of a number
    int subtractProductAndSum(int n) {
        // Initializing variables for multiplication, individual digits, and sum
        int mul = 1;
        int num = 0;
        int sum = 0;

        // Loop to extract digits and perform multiplication and addition
        while (n > 0) {
            num = n % 10;
            mul *= num;   // Multiply the digit to the product
            sum += num;   // Add the digit to the sum
            n = n / 10;   // Remove the last digit
        }

        // Returning the result of subtraction
        return mul - sum;
    }
};

int main() {
    Solution solution;
    std::cout << solution.subtractProductAndSum(123) << std::endl;
    return 0;
}
```

### Java

```java
class Solution {
    // Function to subtract the product and sum of digits of a number
    public int subtractProductAndSum(int n) {
        // Initializing variables for multiplication, individual digits, and sum
        int mul = 1;
        int num = 0;
        int sum = 0;

        // Loop to extract digits and perform multiplication and addition
        while (n > 0) {
            num = n % 10;
            mul *= num;   // Multiply the digit to the product
            sum += num;   // Add the digit to the sum
            n = n / 10;   // Remove the last digit
        }

        // Returning the result of subtraction
        return mul - sum;
    }
}
```

### Python

```python
class Solution:
    # Function to subtract the product and sum of digits of a number
    def subtractProductAndSum(self, n: int) -> int:
        # Initializing variables for multiplication, individual digits, and sum
        mul = 1
        num = 0
        sum = 0

        # Loop to extract digits and perform multiplication and addition
        while n > 0:
            num = n % 10
            mul *= num   # Multiply the digit to the product
            sum += num   # Add the digit to the sum
            n //= 10     # Remove the last digit

        # Returning the result of subtraction
        return mul - sum
```

### Python3

```python
class Solution:
    # Function to subtract the product and sum of digits of a number
    def subtractProductAndSum(self, n: int) -> int:
        # Initializing variables for multiplication, individual digits, and sum
        mul = 1
        num = 0
        sum = 0

        # Loop to extract digits and perform multiplication and addition
        while n > 0:
            num = n % 10
            mul *= num   # Multiply the digit to the product
            sum += num   # Add the digit to the sum
            n //= 10     # Remove the last digit

        # Returning the result of subtraction
        return mul - sum
```

### C

```c
#include <stdio.h>

// Function to subtract the product and sum of digits of a number
int subtractProductAndSum(int n) {
    // Initializing variables for multiplication, individual digits, and sum
    int mul = 1;
    int num = 0;
    int sum = 0;

    // Loop to extract digits and perform multiplication and addition
    while (n > 0) {
        num = n % 10;
        mul *= num;   // Multiply the digit to the product
        sum += num;   // Add the digit to the sum
        n = n / 10;   // Remove the last digit
    }

    // Returning the result of subtraction
    return mul - sum;
}

int main() {
    printf("%d\n", subtractProductAndSum(123));
    return 0;
}
```

### C#

```csharp
public class Solution {
    // Function to subtract the product and sum of digits of a number
    public int SubtractProductAndSum(int n) {
        // Initializing variables for multiplication, individual digits, and sum
        int mul = 1;
        int num = 0;
        int sum = 0;

        // Loop to extract digits and perform multiplication and addition
        while (n > 0) {
            num = n % 10;
            mul *= num;   // Multiply the digit to the product
            sum += num;   // Add the digit to the sum
            n = n / 10;   // Remove the last digit
        }

        // Returning the result of subtraction
        return mul - sum;
    }
}
```

### JavaScript

```javascript
class Solution {
    // Function to subtract the product and sum of digits of a number
    subtractProductAndSum(n) {
        // Initializing variables for multiplication, individual digits, and sum
        let mul = 1;
        let num = 0;
        let sum = 0;

        // Loop to extract digits and perform multiplication and addition
        while (n > 0) {
            num = n % 10;
            mul *= num;   // Multiply the digit to the product
            sum += num;   // Add the digit to the sum
            n = Math.floor(n / 10);   // Remove the last digit
        }

        // Returning the result of subtraction
        return mul - sum;
    }
}

const solution = new Solution();
console.log(solution.subtractProductAndSum(123));
```

### TypeScript

```typescript
class Solution {
    // Function to subtract the product and sum of digits of a number
    subtractProductAndSum(n: number): number {
        // Initializing variables for multiplication, individual digits, and sum
        let mul = 1;
        let num = 0;
        let sum = 0;

        // Loop to extract digits and perform multiplication and addition
        while (n > 0) {
            num = n % 10;
            mul *= num;   // Multiply the digit to the product
            sum += num;   // Add the digit to the sum
            n = Math.floor(n / 10);   // Remove the last digit
        }

        // Returning the result of subtraction
        return mul - sum;
    }
}

const solution = new Solution();
console.log(solution.subtractProductAndSum(123));
```