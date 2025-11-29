## Basic Operations

as stated in the rough notes there are some operations that can be performed on the strings below is the list of all of them:
```
hi = "hello there"
name = "seth"

print(hi + " " + name)   #concatenation
>>>hello there seth

print(hi * 3)   #repetition
>>>hello therehello therehello there

print('h' in hi + "\n")    #membership
print('h' not in hi)
>>>True
>>>False

print(hi[0])   #indexing
>>>h

print(hi[1:4])    #slicing
>>>ell

print(hi == name + "\n")   #comparing
print(hi > name)
>>>False
>>>True
```

## Built-in functions

these are all the functions that can be used on/with strings. strings also have built-in functions:
```
print(len(hi))   #gives the length of the string
>>>11

print(str(123))   #prints the given data as a string
>>>123

print(list(hi))
>>>['h', 'e', 'l', 'l', 'o', ' ', 't', 'h', 'e', 'r', 'e']
```

## Transformations

the commands that are listed below are used for string transformation:
```
print(hi.upper())   #transforms all the substrinngs to UC
>>>HELLO THERE

print(hi.lower())   #transforms all the substrings to LC
>>>hello there

print(hi.title())
>>>Hello There

print(hi.capitalize()) #transforms the 0 of the substring to UC
>>>Hello there

print(hi.swapcase())  #transforms UC to LC and vice versa
>>>HELLO THERE
```

## Querying

the commands below are the querying methods for the string
```
print(hi.find("lo"))
>>>3

print(hi.index("lo"))
>>>3

print(hi.count("l"))
>>>2

print(hi.startswith("he"))
>>>True

print(hi.endswith("re"))
>>>True
```

the main difference between `.find()` and `.index()` is we use `.find()` when we are uncertain whether the element exists in the string or not if not it returns -1. we use `.index()` when we are certain that the element doesnt exist in the string and will give error.

## Formatting

the commands listed below are used for formatting string/s:
```
print(hi.center(20, '*'))
>>>****hello there*****

print(hi.ljust(15, '-'))
>>>hello there****

print(hi.rjust(15, '-'))
>>>****hello there

print(hi.zfill(15))
>>>0000hello there
```

## Splitting and joining

the below ones are for splitting and joining strings
```
print(hi.split())
>>>['hello', 'there']

print(hi.split("t"))
>>>['hello ', 'here']

ho = "hello\nthere"
print(ho.splitlines())
>>>['hello', 'there']

print('-'.join(hi))
>>>h-e-l-l-o- -t-h-e-r-e
```

## Strip/Trim

the ones listed below are on how to trim/strip
```
hp = "  hello there  "
print(hp.strip())
>>>hello there

print(hi.lstrip("hello "))
>>>there

print(hi.rstrip(" there"))
>>>hello
```

## Replacement

this one is for replacement
```
print(hi.replace("l", "L"))
>>>heLLo there
```

## String Verification

the ones below are used to check whether the characters in the string are of a certain datatype or not; or a type in general:
```
print(hi.isalnum())
>>>False

hk = "hello"
print(hk.isalpha())
>>>True

print(hi.isdigit())
>>>False

print(hi.isdecimal())
>>>False

print(hi.isspace())
>>>false

print(hi.islower())
>>>True

print(hi.isupper())
>>>False

print(hi.isidentifier())
>>>False

print("HelloWorld".isidentifier())
>>>True

print(hi.isprintable())
>>>True

print(hi.istitle())
>>>False

hx = "Hello There"
print(hx.istitle())
>>>True

print(hi.isascii())
>>>True
```

## Other methods

these two are some of the other methods that can be performed on the string:
```
print(name\tage.exapndtabs(4))
>>>name    age

print("hello".encode())
>>>b'hello'

print(b'hello'.decode())
>>>hello
```

the `.expandtabs()` will replace `\t` with the number of spaces specified in the (4).
the `.encode()` converts the string from a `str` to `bytes`, `b` indicates its a byte string.
the `.decode()` does the opposite of `.encode()`