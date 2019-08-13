## Statement
There was a set of cards with numbers from 1 to N. One of the card is now lost. Determine the number on that lost card given the numbers for the remaining cards.

Given a number N, followed by N − 1 integers representing the numbers on the remaining cards (distinct integers in the range from 1 to N). Find and print the number on the lost card

```
Example input
5
3
5
2
1

Example output
4

```

```
n = int(input())
for i in range(1,n+1):
  alist.append(i)
for j in range(1,n):
  a = int(input())
  if a in alist:
    alist.remove(a)
print (alist)
    
  (or)
  
Model Solution


  n = int(input())

cards_sum = 0
for i in range(1, n + 1):
  cards_sum += i

for i in range(n - 1):
  cards_sum -= int(input())

print(cards_sum)
```
