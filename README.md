# Sum of two Integers
## https://leetcode.com/problems/sum-of-two-integers

Calculate the sum of two integers a and b, but you are not allowed to use the operator + and -.

Example 1:

Input: a = 1, b = 2
Output: 3
Example 2:

Input: a = -2, b = 3
Output: 1

# Implementation :
```java
class Solution {
    public int getSum(int a, int b) {
        while(b != 0) {
            int carry = a & b;
            a = a ^ b;
            b = carry << 1;
        }
        return a;
    }
}
```
# References :
1. https://www.youtube.com/watch?v=qq64FrA2UXQ
2. https://www.programcreek.com/2015/07/leetcode-sum-of-two-integers-java
