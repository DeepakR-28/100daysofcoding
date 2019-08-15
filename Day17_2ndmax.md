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

num = int(input())
alist = []
alist.append(int(input()))
sorted(alist)
i = 0
maximum = alist[0]
while(i>=len(alist)-1):
  if(alist[i+1]>alist[i]):
    maximum = alist[i+1]
  else:
    i = i+1
print (maximum)
```
