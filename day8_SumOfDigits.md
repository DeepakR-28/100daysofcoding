## Given a three-digit number. Find the sum of its digits.

```
Example input
123

Example output
6

```

```
Code
a = int(input())
b = a
dig_sum=0
while(b !=0):
  rem = b % 10
  dig_sum = dig_sum + rem
  b = b // 10
  
print (dig_sum)
```
