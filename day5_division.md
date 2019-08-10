## N students take K apples and distribute them among each other evenly. The remaining (the indivisible) part remains in the basket. How many apples will each single student get? How many apples will remain in the basket?

```
Example input
6
50

Example output
8
2

```

```
Code
n = int(input())
k = int(input())
   
print(k // n)   # example of integer division
print(k % n)    # example of remainder calculation 
```

