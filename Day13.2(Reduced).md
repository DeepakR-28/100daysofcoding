## JugsMugsPugs LITE
Write a program that receives a number on the input.
  - If the number is a multiple of 3, it prints "Jugs". 
  - If the number is a multiple of 5, it prints "Mugs".
  - If the number is a multiple of 7, it prints "Pugs".

  - If the number is a multiple of both 3 and 5, it prints "JugsMugs".
  - If the number is a multiple of both 3 and 7, it prints "JugsPugs".
  - If the number is a multiple of both 5 and 7, it prints "MugsPugs".
  - If the number is a multiple of both 3, 5 and 7, it prints "JugsMugsPugs".

Otherwise, it prints the number.

```
INPUT 
15

OUTPUT
JugsMugs

INPUT 
21

OUTPUT
JugsPugs


INPUT 
105

OUTPUT 
JugsMugsPugs

```

```
Code
number = int(input())
j = "Jugs"
m = "Mugs"
p = "Pugs"
if(number%3==0):
  print(j)
if(number%5==0):
  print(m)
if(number%7==0):    
  print(p)
if(number%3!=0 and number%5!=0 and number%7!=0):
  print(number)

```
