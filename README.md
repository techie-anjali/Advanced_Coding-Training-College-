  Problem 1: Cyclic Substring Maximum Sum
Description:
Find the maximum sum of a cyclic substring in a given array/string.
 
 
 Algorithm Steps
Duplicate string → t = s + s (to handle circular substrings)
Use two pointers (left, right) for sliding window
Maintain a HashSet to ensure unique characters
If:
Character already exists OR
Window size exceeds n
→ shrink window from left
Add current character and update sum
Track maximum sum

Character weight:
value = ch - 'a' + 1
Maintain:
currentSum → current window sum
maxSum → final answer
 Complexity Analysis
Time Complexity: O(n)
Space Complexity: O(1) (since at most 26 characters)


/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
 
  
  Problem 2: Array Transformation Cost Minimization

Description:
Convert all elements of an array to the same value using operations:

A[i] → A[i] + K OR A[i] - K

Find minimum number of operations.

Approach:

Check feasibility using modulo condition

(A[i] - A[0]) % K == 0
Sort the array
Choose median to minimize operations

Count operations:
|A[i] - median| / K

Time Complexity: O(n log n)
Space Complexity: O(1)
