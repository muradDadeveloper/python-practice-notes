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
