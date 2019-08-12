## JugsMugsPugs Plus
Write a program that receives a number on the input.

  - If the number is a multiple of 3, or it contains digit 3, it prints "Jugs". 
  - If the number is a multiple of 5, or it contains digit 5, it prints "Mugs".
  - If the number is a multiple of 7, or it contains digit 7, it prints "Pugs".

Otherwise, it prints the number.

SPECIAL REQUIREMENT: 
Try and limit the number of conditional statements to not more than 4. 
And use only one print statement.

```
INPUT 
73 
OUTPUT
JugsPugs

INPUT 
51  

OUTPUT
JugsMugs


INPUT 
105

OUTPUT 
JugsMugsPugs
```

```
Code
num = int(input())
digit_1 = '3'
digit_2 = '5'
digit_3 = '7'
var = ''
if(num%3==0 or digit_1 in str(num)):
  var = var+'Jugs'
if(num%5==0 or digit_2 in str(num)):
  var = var + 'Mugs'
if(num%7==0 or digit_3 in str(num)):
  var = var + 'Pugs'
print(var)

```
