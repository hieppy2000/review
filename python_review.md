# Slicing:

```
- reverse string:
  'hello world'[::-1]
  >>'dlrow olleh'
```

```
fruit = "banana"
fruit[:3]
>>'ban'

fruit[3:]
>>output: 'ana'
```

# Convert First word in the line to Capital Letter:
```
"hello world".title()
>>’Hello World'
```
```
import string
s = "this is a list"
string.capwords(s)
>>’This Is A List'
```

# tuple vs list: tuple have structure, lists have order
    - list is in sequences, list can be modified
    - tuple you can not modify, if you want to modify tuple, you have change to list then modify it
    - tuple have structure for example (42, 11) # page number, line number
