# 1 - Set In Dart

Set is a unique collection of items. You cannot store duplicate values in the Set. It is unordered, so it can be faster than lists while working with a large amount of data. Set is useful when you need to store unique values without considering the order of the input. E.g., fruits name, months name, days name, etc. It is represented by Curley Braces`{}`.

Info

Note: The list allows you to add duplicate items, but the Set doesn’t allow it.

Syntax

```
Set <variable_type> variable_name = {};
```

# 2 - How To Create A Set In Dart

You can create a Set in Dart using the Set type annotation. Here Set<String> means only text is allowed in the Set.

```
void main()
{
  Set<String> fruits = {"Apple", "Orange", "Mango"};

  print(fruits);
}
```

**OUTPUT**
```
{Apple, Orange, Mango}
```

# 3 - first
To get first value of Set.

```
void main() 
{
  // declaring fruits as Set
  Set<String> fruits = {"Apple", "Orange", "Mango", "Banana"};

  // using different properties of Set
  print("First Value is ${fruits.first}");
}
```

**OUTPUT**
```
First Value is Apple
```

# 4 - last

To get last value of Set.

```
void main() 
{
  // declaring fruits as Set
  Set<String> fruits = {"Apple", "Orange", "Mango", "Banana"};

  // using different properties of Set
  print("Last Value is ${fruits.last}");
}
```

**OUTPUT**
```
Last Value is Banana
```

# 5 - isEmpty

Return true or false.

```
void main() 
{
  // declaring fruits as Set
  Set<String> fruits = {"Apple", "Orange", "Mango", "Banana"};

  // using different properties of Set
  print("Is fruits empty? ${fruits.isEmpty}");
}
```

**OUTPUT**
```
Is fruits empty? false
```

# 6 - isNotEmpty

Return true or false.

```
void main() 
{
  // declaring fruits as Set
  Set<String> fruits = {"Apple", "Orange", "Mango", "Banana"};

  // using different properties of Set
  print("Is fruits not empty? ${fruits.isNotEmpty}");
}
```

**OUTPUT**
```
Is fruits not empty? true
```

# 7 - length

It returns the length of the Set.

```
void main() 
{
  // declaring fruits as Set
  Set<String> fruits = {"Apple", "Orange", "Mango", "Banana"};

  // using different properties of Set
  print("The length of fruits is ${fruits.length}");
}
```

**OUTPUT**
```
The length of fruits is 4
```

# 8 - contains

If you want to see whether the Set contains specific items or not, you can use the contains method, which returns true or false.

```
void main() 
{
  // declaring fruits as Set
  Set<String> fruits = {"Apple", "Orange", "Mango", "Banana"};

  // using different properties of Set
  print(fruits.contains("Mango"));
  print(fruits.contains("Lemon"));
}
```

**OUTPUT**
```
true
false
```

# 9 - add

Add one element to Set.

```
void main() 
{
  Set<String> fruits = {"Apple", "Orange", "Mango"};
  
  fruits.add("Lemon");
  fruits.add("Grape");
  
  print("After Adding Lemon and Grape: $fruits");
}
```

**OUTPUT**
```
After Adding Lemon and Grape: {Apple, Orange, Mango, Lemon, Grape}
```

# 10 - remove

Removes one element from Set.

```
void main() 
{
  Set<String> fruits = {"Apple", "Orange", "Mango"};
  
  fruits.remove("Apple");
  
  print("After Removing Apple: $fruits");
}
```

**OUTPUT**
```
After Removing Apple: {Orange, Mango}
```

# 11 - addAll

Insert the multiple values to the given Set.

```
void main() 
{
  Set<String> fruits = {"Apple", "Orange", "Mango"};
  
  fruits.addAll(["Lemon", "Grape"]);

  print("After Adding Lemon and Grape: $fruits");
}
```

**OUTPUT**
```
After Adding Lemon and Grape: {Apple, Orange, Mango, Lemon, Grape}
```

# 12 - Printing All Values In Set

You can print all Set items by using loops. Click here if you want to learn loop in dart.

```
void main() 
{
  Set<String> fruits = {"Apple", "Orange", "Mango"};
  
  for(String element in fruits)
  {    
    print(element);
  }
}
```

**OUTPUT**
```
Apple
Orange
Mango
```

# 13 - clear

Removes all elements from the Set.

```
void main() 
{
  Set<String> fruits = {"Apple", "Orange", "Mango"};
  
  // to clear all items
  fruits.clear();

  print(fruits);
}
```

**OUTPUT**
```
{}
```

# 14 - difference

Creates a new Set with the elements of this that are not in other.

```
void main() 
{
  Set<String> fruits1 = {"Apple", "Orange", "Mango"};
  Set<String> fruits2 = {"Apple", "Grapes", "Banana"};

  final differenceSet = fruits1.difference(fruits2);

  print(differenceSet);
}
```

**OUTPUT**
```
{Orange, Mango}
```

# 15 - elementAt

Returns the index value of element.

```
void main() 
{
  Set<String> days = {"Sunday", "Monday", "Tuesday"};
  
  // index starts from 0 so 2 means Tuesday
  print(days.elementAt(2));
}
```

**OUTPUT**
```
Tuesday
```

# 16 - intersection

Find common elements in two sets.

```
void main() 
{
  Set<String> fruits1 = {"Apple", "Orange", "Mango"};
  
  Set<String> fruits2 = {"Apple", "Grapes", "Banana"};

  final intersectionSet = fruits1.intersection(fruits2);

  print(intersectionSet);
}
```

**OUTPUT**
```
{Apple}
```