# Dynamic Programming

## 1. Basic Content

The five steps of dynamic programming problems:

​	(1)Determine dp array and the meaning of index

​	(2)Determine the recurrence formula

​	(3)Initialize dp array

​	(4)Determine traversal order

​	(5)Derive dp array with examples

## 2.Fibonacci Number-LC509

​	(1)Determine dp array: dp[i] which means the Fibonacci Numeber of number i.

​	(2)Determine the recurrence formula: F(n) = F(n-1) + F(n-2)

​	(3)dp[0] = 0, dp[1] = 1	

```python
def fib(n:int)->int:
    if n <= 1:
        return n
    dp =[0] * (n+1)
    dp[0] = 0
    dp[1] = 1
    for i in range(2,n+1):
        dp[i] = dp[i-1] + dp[i-2]
    return dp[n]
```



​	

