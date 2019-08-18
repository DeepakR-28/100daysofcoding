## First Statement
Given a list of numbers, find and print all its elements with even indices (i.e. A[0], A[2], A[4], ...).

## Second Statement

Statement
Given a list of numbers, print all its even elements. Use a for-loop that iterates over the list itself and not over its indices. That is, don't use range()

## Third Statement

Statement
Given a list of numbers, find and print all its elements that are greater than their left neighbor.

## Fourth Statement

Statement
Given a list of non-zero integers, find and print the first adjacent pair of elements that have the same sign. If there is no such pair, print 0.

## Examples
```
Example For 1st Statement

Example input
5 6 7 8 9

Example output
5 7 9
```

```
Example For Second Statement

Statement
Given a list of numbers, print all its even elements. Use a for-loop that iterates over the list itself and not over its indices. That is, don't use range()

```

```
Example input
1 5 2 4 3

Example output
5 4
```

```
Example input #1
-1 2 3 -1 -2

Example output #1
2 3

Example input #2
1 -3 4 -2 1

Example output #2
0

```

## Source Code

```
Source Code for First  Statement

a = [int(s) for s in input().split()]
# Print a value:
# print(a)
print(a[0:len(a):2])

```

```
Source Code For 2nd Statement

a = [int(s) for s in input().split()]
# Print a value:
# print(a)
alist = []
for i in  a:
  if i % 2 ==0:
    print(i)

```

```
Source Code for 3rd Statement

a = [int(s) for s in input().split()]
# Print a value:
# print(a)
for i in range(1,len(a)):
  if( a[i]>a[i-1]):
    print(a[i])
    
```

```
Source Code for 4th

a = [int(s) for s in input().split()]
# Print a value:
# print(a)
flag = 0
for i in range(0,len(a)-1):
  if(a[i] > 0 and a[i+1] > 0):
    print(a[i] , a[i+1])
    flag = 1
    break
  elif(a[i] < 0 and a[i+1] < 0):
    print(a[i] , a[i+1])
    flag = 1
    break
if (flag != 1):
  print("0")

```
