## Statement
In mathematics, the factorial of an integer n, denoted by n! is the following product:

n! = 1 × 2 × … × n

For the given integer n calculate the value 

1! + 2! + 3! + ... + n!

Try to discover the solution that uses only one for-loop. And don't use math module in this exercise.

```
Example input
4

Example output
33
```

```
Source Code

num = int(input())
fact=1
ans=0
for Dig_Fact in range(1,num+1):
  fact*=Dig_Fact
  ans = ans+fact
print(ans) 
```
