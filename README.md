  Problem 1: Cyclic Substring Maximum Sum
Description:
Find the maximum sum of a cyclic substring in a given array/string.
Approach:
Used variation of Kadane’s Algorithm
Handled circular nature by combining:
Normal max subarray
Total sum - min subarray

Time Complexity: O(n)
Space Complexity: O(1)

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
