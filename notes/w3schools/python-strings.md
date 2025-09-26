## Looping Through a String

Since strings are arrays, we can loop through the characters in a string, with a for loop.

``` Python

#/usr/bin/python3

for x in "banana":
print(x)

```

## String Length

To get the length of a string, use the len() function.

```Python

#/usr/bin/python3

a = "Hello, World!"
print(len(a))

```

## Check String

To check if a certain phrase or character is present in a string.

``` Python
#/usr/bin/python3

txt = "The best things in life are free!"  
print("free" in txt)
```

``` Python
#/usr/bin/python3

txt = "The best things in life are free!"  
if "free" in txt:  
  print("Yes, 'free' is present.")
```


## Check if NOT

To check if a certain phrase or character is NOT present in a string, we can use the keyword `not in`.

``` Python
#/usr/bin/python3

txt = "The best things in life are free!"  
print("expensive" not in txt)
```

``` Python
#/usr/bin/python3

txt = "The best things in life are free!"  
if "expensive" not in txt:  
  print("No, 'expensive' is NOT present.")
```

## Slice From the Start & End

By leaving out the start index, the range will start at the first character and by leaving out the end index, the range will go to the end:

```Python
b = "Hello, World!"
print(b[:5])

c = "Hello, World!"
print(b[2:])
```

## Slice To the End

By leaving out the end index, the range will go to the end:

```Python
b = "Hello, World!"
print(b[2:])
```

## Remove Whitespace

Whitespace is the space before and/or after the actual text, and very often you want to remove this space.

```Python
a = " Hello, World! "
print(a.strip())
```

## Replace String

The replace() method replaces a string with another string:

```Python
a = "Hello, World!"
print(a.replace("H", "J"))
```

## Split String

The split() method returns a list where the text between the specified separator becomes the list items.

```Python
a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!'] 
```

## Placeholders and Modifiers

A placeholder can contain variables, operations, functions, and modifiers to format the value. 

```Python
price = 59
txt = f"The price is {price} dollars"
print(txt)
```