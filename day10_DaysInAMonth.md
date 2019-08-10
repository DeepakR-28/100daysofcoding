## Given a month - an integer from 1 to 12, print the number of days in it in the year 2017.

```
Example input #1
1
(January)

Example output #1
31

Example input #2
2
(February)
```

```
Code

a= int(input())
if(a==2):
  print("28")
elif((a<8 and a%2 !=0) or (a>7 and a%2 == 0) ):
  print("31")
else:
  print("30")

```
