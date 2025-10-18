## Python Tuples

- Tuples are used to store multiple items in a single variable.
- Tuple is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Set, and Dictionary, all with different qualities and usage.
- A tuple is a collection which is ordered and unchangeable.
- Tuples are written with round brackets.

## Tuple Items

- Tuple items are ordered, unchangeable, and allow duplicate values.


## Basic example

``` Python
thistuple = ("apple", "banana", "cherry", "apple", "cherry")
print(thistuple)
```

## Tuple Length

Use `len()` function to determine how many items a tuple has.
``` Python
thistuple = ("apple", "banana", "cherry")
print(len(thistuple))
```

## Create Tuple with one Item

To create a tuple with only one item, you have to add a comma after the item, otherwise Python will not recognize it as a tuple.

``` Python
thistuple = ("apple",)
print(type(thistuple))
```

## The tuple() Constructor

It is also possible to use the tuple() constructor to make a tuple.

``` Python
thistuple = tuple(("apple", "banana", "cherry"))
print(thistuple)
```
## Ranges of Indexes 

You can specify a range of indexes by specifying where to start and where to end the range. When specifying a range, the return value will be a new tuple with the specified items.

``` Python
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[2:5])
```
- This example returns the items from the beginning to, but NOT included, "kiwi":

``` Python
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[:4])
```
- This example returns the items from "cherry" and to the end:

``` Python
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[2:])
```

## Check if Item Exists

To determine if a specified item is present in a tuple use the in keyword

``` Python
thistuple = ("apple", "banana", "cherry")
if "apple" in thistuple:
    print("Yes, 'apple' is in the fruits tuple") 
```

## Change Tuple Values

Once a tuple is created, you cannot change its values. Tuples are unchangeable, or immutable as it also is called.

``` Python
x = ("apple", "banana", "cherry")
y = list(x)
y[1] = "kiwi"
x = tuple(y)

print(x) 
```

## Add Items

Since tuples are immutable, they do not have a built-in append() method, but there are other ways to add items to a tuple.

1. Convert into a list: Just like the workaround for changing a tuple, you can convert it into a list, add your item(s), and convert it back into a tuple.

``` Python
thistuple = ("apple", "banana", "cherry")
y = list(thistuple)
y.append("orange")
thistuple = tuple(y)
```
2. Add tuple to a tuple. You are allowed to add tuples to tuples, so if you want to add one item, (or many), create a new tuple with the item(s), and add it to the existing tuple:

``` Python
thistuple = ("apple", "banana", "cherry")
y = ("orange",)
thistuple += y

print(thistuple)
```
3. Tuples are unchangeable, so you cannot remove items from it, but you can use the same workaround as we used for changing and adding tuple items:

``` Python
thistuple = ("apple", "banana", "cherry")
y = list(thistuple)
y.remove("apple")
thistuple = tuple(y)
```
Or you can delete the tuple completely:

``` Python
thistuple = ("apple", "banana", "cherry")
del thistuple
print(thistuple)
```

## Loop Through the Index Numbers 

You can also loop through the tuple items by referring to their index number.
Use the range() and len() functions to create a suitable iterable.

``` Python
thistuple = ("apple", "banana", "cherry")
for i in range(len(thistuple)):
  print(thistuple[i]) 
```

## Join Two Tuples 

To join two or more tuples you can use the + operator:

``` Python
tuple1 = ("a", "b" , "c")
tuple2 = (1, 2, 3)

tuple3 = tuple1 + tuple2
print(tuple3) 
```

If you want to multiply the content of a tuple a given number of times, you can use the * operator:

``` Python
fruits = ("apple", "banana", "cherry")
mytuple = fruits * 2

print(mytuple) 
```