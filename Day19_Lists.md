## Statements

## First Statement


Statement
Given a list of numbers, determine and print the number of elements that are greater than both of their neighbors.

The first and the last items of the list shouldn't be considered because they don't have two neighbors.

## Second Statement

Statement
Given a list of numbers with all elements sorted in ascending order, determine and print the number of distinct elements in it.

## Third Statement

Statement
Given a list of numbers, swap adjacent elements in each pair (swap A[0] with A[1], A[2] with A[3], etc.). Print the resulting list. If a list has an odd number of elements, leave the last element intact.

## Fourth Statement

Statement
Given a list of distinct numbers, swap the minimum and the maximum and print the resulting list.


## Examples

```
Example For statement 1

Example input
1 5 1 5 1

Example output
2

```

```
Example For statement 2
Example input
1 2 2 3 3 3

Example output
3

```
```
Example For statement 3

Example input
1 2 3 4 5

Example output
2 1 4 3 5

```

```
Example for statement 4

Example input
3 4 5 2 1

Example output
3 4 1 2 5

```



## Source Codes

```
Source Code for First statement

a = [int(s) for s in input().split()]
# Print a value:
# print(a)
count = 0
for i in range(1,len(a)-1):
  if(a[i]>a[i-1] and a[i]>a[i+1]):
    count+=1
print(count)
```

```
Source Code for statement 2

# Read a list of integers:
a = [int(s) for s in input().split()]
# Print a value:
# print(a)
alist = []
count = 0
for i in a:
  if(i not in alist):
    alist.append(i)
print(len(alist))

```

```
Source Code for statement 3

# Read a list of integers:
a = [int(s) for s in input().split()]
# Print a value:
# print(a)
b = len(a)
i = 0
alist = a[0::2]
blist = a[1::2]
clist=[]
flag=0
if(len(a)%2!=0):
  flag=1
for i in range(0,len(blist)):
  clist.append(blist[i])
  clist.append(alist[i])
if(flag):
  clist.append(a[len(a)-1])
print(clist)

```

```
Source Code for statement 4

# Read a list of integers:
a = [int(s) for s in input().split()]
max , min = a.index(max(a)),a.index(min(a))
a[min], a[max] = a[max],a[min]
print(a)

```


