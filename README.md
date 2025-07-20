# Interview

Q1: Longest Consecutive Sequence
Write a function that takes an array of integers and returns the longest sequence of consecutive
numbers in the array.

#Solution
see source code
⏱ Time Complexity: O(n)
🗂 Space Complexity: O(n)





Q3: Debugging Fibonacci Function
The following Python function is supposed to return the n-th Fibonacci number, but it contains
an error.
Task:
● Identify the issue in the function.
● Fix the function so that it correctly calculates Fibonacci numbers.

def fibonacci(n):
if n == 0:
return 0
elif n == 1:
return 1
else:
return fibonacci(n - 1) + fibonacci(n - 2)

Steps to Follow:
1. Identify the bug in the function.
2. Fix the function to compute Fibonacci numbers correctly.
3. Ensure the function runs efficiently for larger values of n.

#Solution
While logically correct, this recursive implementation has two major problems:
Exponential Time Complexity: It recalculates the same Fibonacci numbers many times, leading to O(2^n) time complexity.
Stack Overflow Risk: For large n, it could hit Python's recursion depth limit.

The iterative approach is generally best for this problem as it:
Runs in O(n) time
Uses O(1) space
Doesn't risk stack overflow
Is simple and easy to understand
