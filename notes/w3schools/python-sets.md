## Set
 
Sets are used to store multiple items in a single variable. Set is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Tuple, and Dictionary, all with different qualities and usage. A set is a collection which is unordered, unchangeable*, and unindexed.

## Set Items 

Set items are unordered, unchangeable, and do not allow duplicate values. Sets cannot have two items with the same value.

## Get the Length of a Set

To determine how many items a set has, use the len() function.

## Add Items

``` Python
thisset = {"apple", "banana", "cherry"}
thisset.add("orange")

print(thisset) 
```

## Add Set

``` Python
thisset = {"apple", "banana", "cherry"}
tropical = {"pineapple", "mango", "papaya"}

thisset.update(tropical)
print(thisset) 
```

## Add any iterable 

``` Python
thisset = {"apple", "banana", "cherry"}
mylist = ["kiwi", "orange"]

thisset.update(mylist)
print(thisset) 
```

## Remove item

``` Python
thisset = {"apple", "banana", "cherry"}
thisset.remove("banana")

print(thisset) 
```

`clear()` method empties the set:

``` Python
thisset = {"apple", "banana", "cherry"}
thisset.clear()

print(thisset) 
```

## Loop Items

You can loop through the set items by using a for loop:


``` Python
thisset = {"apple", "banana", "cherry"}

for x in thisset:
  print(x) 
```

## Join Sets

There are several ways to join two or more sets in Python.

- The `union()` and `update()` methods joins all items from both sets.
- The `intersection()` method keeps ONLY the duplicates.
- The `difference()` method keeps the items from the first set that are not in the other set(s).
- The `symmetric_difference()` method keeps all items EXCEPT the duplicates.

## Union

The union() method returns a new set with all items from both sets.

``` Python
set1 = {"a", "b", "c"}
set2 = {1, 2, 3}

set3 = set1.union(set2)
print(set3) 
```

You can use the | operator instead of the union() method, and you will get the same result.

``` Python
set1 = {"a", "b", "c"}
set2 = {1, 2, 3}

set3 = set1 | set2
print(set3) 
```