## INTERVIEW GRADE PROBLEM
JugsMugsPugs Special
SPECIAL REQUIREMENT: 
Try and limit the number of conditional statements to not more than two. 
This requires some advanced Python language knowledge. I don't expect everyone  
to be able to complete this.

Write a program that receives a number on the input and prints values from 1 to that number subjected to the conditions below. 
It also should receive another value 'rev' (either 0 or 1) on the input. 

For every number in the given range,   
- If the number is a multiple of 3, or it contains digit 3, it prints "Jugs".   
- If the number is a multiple of 5, or it contains digit 5, it prints "Mugs".  
- If the number is a multiple of 7, or it contains digit 7, it prints "Pugs".

- If the number is a multiple of both 3 and 5, it prints "JugsMugs".        
  - also if number contains 3 and 5, it prints "JugsMugs"  
- If the number is a multiple of both 3 and 7, it prints "JugsPugs".        
  - also if number contains 3 and 7, it prints "JugsPugs"
 - If the number is a multiple of 3, 5 and 7, it prints "JugsMugsPugs".
       - also if number contains 3, 5 and 7, it prints "JugsMugsPugs"

Otherwise, it prints the number.

REVERSE REQUIREMENT:
If the boolean 'rev' is True (or 1), then reverse the order of printing.    
  - "PugsJugsMugs" for multiples of 3, 5 and 7   
  - "PugsMugs" for multiple of 3 and 7   
  - "MugsJugs" for multiple of 3 and 5    
  - "PugsJugs" for multiple of 5 and 7
  
  ```
  INPUT 
5
False
OUTPUT
1
2
Jugs
4
Mugs
INPUT 
15
True
OUTPUT
1
2
Jugs
4
Mugs
Jugs
Pugs
8
Jugs
Mugs
11
Jugs
Jugs
Pugs
MugsJugs
 ```
 
 ```
 Code
 a = input()
 n int(input())
 rev  = bool(input())
 s = a
 str1=""
 word = ["Jugs" ,"Mugs" ,"Pugs"]
 if rev:
  c=['7','5','3']
  word=["Pugs","Mugs","Jugs"]
 for j in range(1,n+1):
  s = str(j)
  str1=""
  for i in range (3):
    if (j%int(c[i]==0 or c[i] in str(j));
    s= ""
    str1 +=word[i]
   print(s+str1)
   
 ```
