## Given two timestamps of the same day: a number of hours, minutes and seconds for both of the timestamps. The moment of the first 
## timestamp happened before the moment of the second one. Calculate how many seconds passed between them.

```
Example input #1
1
1
1
2
2
2

Example output #1
3661
```
```
Example input #2
1
2
30
1
3
20

Example output #2
50
```
```
Code
a = int(input())
b = int(input())
c = int(input())
d = int(input())
e = int(input())
f = int(input())
x = d*3600 - a*3600
y = e*60  - b*60
z= f-c
p = x+y+z
print(p)
```
