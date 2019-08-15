## Statement
Given a sequence of distinct non-negative integers, where each number is written in a separate line. The sequence ends with 0. Print the second largest element in this sequence. It is guaranteed that the sequence has at least two elements.

```
Example input
1
7
9
0

Example output
7


```

```
Source Code
alist = []
flag = 1
while(flag):
  num = int(input())
  alist.append(num)
  if(num == 0):
    break
  alist.sort(reverse = True)
print(alist[1])
```
