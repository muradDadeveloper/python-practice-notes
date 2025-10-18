## Python Lists

- Lists are used to store multiple items in a single variable. 
- Lists are one of 4 built-in data types in Python used to store collections of data.
- Lists are created using square brackets. 
- List items are ordered, changeable, and allow duplicate values. List items are indexed, the first item has index [0], the second item has index [1] etc. 
- The list is changeable, meaning that we can change, add, and remove items in a list after it has been created.
- Since lists are indexed, lists can have items with the same value.


## List Length

To determine how many items a list has, use the len() function:

``` Python
thislist = ["apple", "banana", "cherry"]
print(len(thislist))
```

## List Items - Data Types

List items can be of any data type:

``` Python
list1 = ["apple", "banana", "cherry"]
list2 = [1, 5, 7, 9, 3]
list3 = [True, False, False]
```

## Check if Item Exists

To determine if a specified item is present in a list use the in keyword:

``` Python
thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list") 
```

## Change a Range of Item Values

``` Python
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"]
thislist[1:3] = ["blackcurrant", "watermelon"]
print(thislist)
```

## Insert Items

To insert a new list item, without replacing any of the existing values, we can use the insert() method.

```Python
thislist = ["apple", "banana", "cherry"]
thislist.insert(2, "watermelon")
print(thislist)
```
## Append Items

To add an item to the end of the list, use the append() method:

``` Python
thislist = ["apple", "banana", "cherry"]
thislist.append("orange")
print(thislist)
```

## Insert Items

To insert a list item at a specified index, use the insert() method.

``` Python
thislist = ["apple", "banana", "cherry"]
thislist.insert(1, "orange")
print(thislist)
```

## Extend List

To append elements from another list to the current list, use the extend() method.

``` Python
thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]
thislist.extend(tropical)
print(thislist)
```

## Add Any Iterable

The extend() method does not have to append lists, you can add any iterable object (tuples, sets, dictionaries etc.).

``` Python
thislist = ["apple", "banana", "cherry"]
thistuple = ("kiwi", "orange")

thislist.extend(thistuple)

print(thislist) 
```

## Remove Specified Index

``` Python
thislist = ["apple", "banana", "cherry"]
thislist.pop(1)
print(thislist)
```
The del keyword also removes the specified index:

``` Python
thislist = ["apple", "banana", "cherry"]
del thislist[0]
print(thislist)
```

The del keyword can also delete the list completely.

``` Python
thislist = ["apple", "banana", "cherry"]
del thislist 
```

## Clear the List

The clear() method empties the list. The list still remains, but it has no content.

``` Python
thislist = ["apple", "banana", "cherry"]
thislist.clear()
print(thislist)
```

## Loop Through a List

You can loop through the list items by using a for loop:

``` Python
thislist = ["apple", "banana", "cherry"]
for x in thislist:
  print(x) 
```

## Using a While Loop

You can loop through the list items by using a while loop. Use the len() function to determine the length of the list, then start at 0 and loop your way through the list items by referring to their indexes. Remember to increase the index by 1 after each iteration.

``` Python
thislist = ["apple", "banana", "cherry"]
i = 0
while i < len(thislist):
  print(thislist[i])
  i = i + 1
```

## Sort List Alphanumerically

List objects have a sort() method that will sort the list alphanumerically, ascending, by default:

``` Python
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort()
print(thislist)
```

## Sort Descending

To sort descending, use the keyword argument reverse = True:

``` Python
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort(reverse = True)
print(thislist)
```
## Case Insensitive Sort

By default the sort() method is case sensitive, resulting in all capital letters being sorted before lower case letters. So if you want a case-insensitive sort function, use str.lower as a key function:

``` Python
thislist = ["banana", "Orange", "Kiwi", "cherry"]
thislist.sort(key = str.lower)
print(thislist)
```

## Copy a List

You can use the built-in List method copy() to copy a list.

``` Python
thislist = ["apple", "banana", "cherry"]
mylist = thislist.copy()
print(mylist)
```

Another way to make a copy is to use the built-in method list().

``` Python
thislist = ["apple", "banana", "cherry"]
mylist = list(thislist)
print(mylist)
```
## Join Two Lists

There are several ways to join, or concatenate, two or more lists in Python. One of the easiest ways are by using the + operator.

``` Python
list1 = ["a", "b", "c"]
list2 = [1, 2, 3]

list3 = list1 + list2
print(list3) 
```
Another way to join two lists is by appending all the items from list2 into list1, one by one:

``` Python
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

for x in list2:
  list1.append(x)

print(list1) 
```
Or you can use the extend() method, where the purpose is to add elements from one list to another list:

``` Python
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

list1.extend(list2)
print(list1) 
```