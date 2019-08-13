## Statement
For the given integer N calculate the following sum:

1³ + 2³ + ... + N³

```
Example input
3

Example output
36

```

```
Source Code

num = int(input())
ans = 0
for val in range(1,num+1):
  ans = ans  + val*val*val
print(ans)
```
