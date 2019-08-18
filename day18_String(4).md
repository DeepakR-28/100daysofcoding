## Statement
Given a string in which the letter h occurs at least twice, reverse the sequence of characters enclosed between the first and last occurrences of it.

```
Example input
In the hole in the ground there lived a hobbit

Example output
In th a devil ereht dnuorg eht ni eloh ehobbit
```

```
Source Code
s = input()
a = s.find('h')
b = s.rfind('h')
rev = s[a:b]
x = rev[::-1]
print(s[:a+1]+str(x)+s[b+1:])

```
