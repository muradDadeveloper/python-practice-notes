## Dictionary
- Dictionaries are used to store data values in key:value pairs.
- A dictionary is a collection which is ordered*, changeable and do not allow duplicates.

## Dictionary Items

- Dictionary items are ordered, changeable, and do not allow duplicates.
- Dictionary items are presented in key:value pairs, and can be referred to by using the key name
- Dictionaries cannot have two items with the same key

## Dictionary Length

``` Python
print(len(thisdict))
```

## The dict() Constructor

It is also possible to use the dict() constructor to make a dictionary.

``` Python
thisdict = dict(name = "John", age = 36, country = "Norway")
print(thisdict)
```

## Accessing Items

You can access the items of a dictionary by referring to its key name, inside square brackets:

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
x = thisdict["model"]
```

There is also a method called get() that will give you the same result:

``` Python
x = thisdict.get("model")
```

## Get Keys

The keys() method will return a list of all the keys in the dictionary.

``` Python
x = thisdict.keys() 
```
The list of the keys is a view of the dictionary, meaning that any changes done to the dictionary will be reflected in the keys list.

``` Python
car = {
"brand": "Ford",
"model": "Mustang",
"year": 1964
}

x = car.keys()
print(x) 

car["color"] = "white"
print(x) 
```

## Get Values

The values() method will return a list of all the values in the dictionary.

``` Python
x = thisdict.values() 
```

## Get Items

``` Python
x = thisdict.items() 
```

## Check if Key Exists

To determine if a specified key is present in a dictionary use the in keyword:

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}

if "model" in thisdict:
  print("Yes, 'model' is one of the keys in the thisdict dictionary") 
```

## Change values

You can change the value of a specific item by referring to its key name:

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["year"] = 2018
```

## Adding Items

Adding an item to the dictionary is done by using a new index key and assigning a value to it:

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["color"] = "red"
print(thisdict)
```

## Update Dictionary

The update() method will update the dictionary with the items from a given argument. If the item does not exist, the item will be added.

The argument must be a dictionary, or an iterable object with key:value pairs.

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.update({"color": "red"})
```

## Removing an Item

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.pop("model")
print(thisdict) 
```
The del keyword removes the item with the specified key name:

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
del thisdict["model"]
print(thisdict) 
```

## Loop through a Dictionary

Usage: 

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
for x in thisdict:
  print(thisdict[x])
```

You can also use the values() method to return values of a dictionary:

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
for x in thisdict.values():
  print(x)
```

You can use the keys() method to return the keys of a dictionary:

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
for x in thisdict.keys():
  print(x)

```

Loop through both keys and values, by using the items() method:

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
for x, y in thisdict.items():
  print(x, y)
```

## Copy a Dictionary

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
mydict = thisdict.copy()
print(mydict)
```

Another way to make a copy is to use the built-in function dict().

``` Python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
mydict = dict(thisdict)
print(mydict) 
```

## Nested Dictionary

A dictionary can contain dictionaries, this is called nested dictionaries:

``` Python
myfamily = {
  "child1" : {
    "name" : "Emil",
    "year" : 2004
  },
  "child2" : {
    "name" : "Tobias",
    "year" : 2007
  },
  "child3" : {
    "name" : "Linus",
    "year" : 2011
  }
} 
```

Or, if you want to add three dictionaries into a new dictionary:

``` Python
child1 = {
  "name" : "Emil",
  "year" : 2004
}
child2 = {
  "name" : "Tobias",
  "year" : 2007
}
child3 = {
  "name" : "Linus",
  "year" : 2011
}

myfamily = {
  "child1" : child1,
  "child2" : child2,
  "child3" : child3
} 
```

## Access Items in Nested Dictionaries

To access items from a nested dictionary, you use the name of the dictionaries, starting with the outer dictionary:

``` Python
myfamily = {
  "child1" : {
    "name" : "Emil",
    "year" : 2004
  },
  "child2" : {
    "name" : "Tobias",
    "year" : 2007
  },
  "child3" : {
    "name" : "Linus",
    "year" : 2011
  }
}

print(myfamily["child2"]["name"])
```

## Loop Through Nested Dictionaries

You can loop through a dictionary by using the items() method like this:

``` Python
for x, obj in myfamily.items():
  print(x)

  for y in obj:
    print(y + ':', obj[y])
```

``` Python

```

``` Python

```

``` Python

```

``` Python

```

``` Python

```

``` Python

```

``` Python

```

``` Python

```