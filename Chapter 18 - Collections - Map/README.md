# 1 - Map In Dart

In a Map, data is stored as keys and values. In Map, each key must be unique. They are similar to HashMaps and Dictionaries in other languages.

# 2 - Create Map In Dart

Here we are creating a Map for String and String. It means keys and values must be the type of String. You can create a Map of any kind as you like.

```
void main()
{  
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital);
}
```

**OUTPUT**

```
{USA: Washington, D.C., India: New Delhi, China: Beijing}

{USA: Washington, D.C., India: New Delhi, China: Beijing}
```

# 3 - Access Value From Key

You can find the value of Map from its key. Here we are printing Washington, D.C. by its key, i.e., USA.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital["USA"]);
}
```

**OUTPUT**
```
Washington, D.C.
```

# 4 - keys

To get all keys.

void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.keys);
}

**OUTPUT**
```
(USA, India, China)
```

# 5 - values

To get all values.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.values);
}
```

**OUTPUT**
```
(Washington, D.C., New Delhi, Beijing)
```

# 6 - isEmpty

Return true or false.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.isEmpty);
}
```

**OUTPUT**
```
false
```

# 7 - isNotEmpty

Return true or false.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.isNotEmpty);
}
```

**OUTPUT**
```
true
```

# 8 - length

It returns the length of the Map.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.length);
}
```

**OUTPUT**
```
3
```

# 9 - Adding Element To Map

If you want to add an element to the existing Map. Here is the way for you:

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  // Adding New Item
  countryCapital['Japan'] = 'Tokio';

  print(countryCapital);
}
```

**OUTPUT**
```
{USA: Washington, D.C., India: New Delhi, China: Beijing, Japan: Tokio}
```

# 10 - Updating An Element Of Map

If you want to update an element of the existing Map. Here is the way for you:

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Nothing',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  // Adding New Item
  countryCapital['USA'] = 'Washington, D.C.';

  print(countryCapital);
}
```

**OUTPUT**
```
{USA: Washington, D.C., India: New Delhi, China: Beijing}
```

# 11 - keys.toList

Convert all Maps keys to List.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Nothing',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.keys.toList());
}
```

**OUTPUT**
```
[USA, India, China]
```

# 12 - values.toList

Convert all Maps values to List.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Nothing',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.values.toList());
}
```

**OUTPUT**
```
[Nothing, New Delhi, Beijing]
```

# 13 - containsKey

Return true or false.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Nothing',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.containsKey("USA"));
}
```

**OUTPUT**
```
true
```

# 14 - containsValue

Return true or false.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  print(countryCapital.containsValue("New Delhi"));
}
```

**OUTPUT**
```
true
```

# 15 - clear

Removes all elements from the Map.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  countryCapital.clear();

  print(countryCapital);
}
```

**OUTPUT**
```
{}
```

# 16 - removeWhere

Removes all elements from the Map if condition is valid.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  countryCapital.removeWhere((key, value) => key == 'USA');

  print(countryCapital);
}
```

**OUTPUT**
```
{India: New Delhi, China: Beijing}
```

# 17 - remove

Suppose you want to remove an element of the existing Map. Here is the way for you:

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  countryCapital.remove("USA");
  
  print(countryCapital);
}
```

**OUTPUT**
```
{India: New Delhi, China: Beijing}
```

# 18 - Looping Over Element Of Map

You can use any loop in Map to print all keys/values or to perform operations in its keys and values.

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

   // Loop Through Map
  for(MapEntry element in countryCapital.entries){
    print('Key is ${element.key}, value ${element.value}');
  }
}
```

**OUTPUT**
```
Key is USA, value Washington, D.C.
Key is India, value New Delhi
Key is China, value Beijing
```

# 19 - Looping In Map Using For Each

Looping In Map Using For Each

```
void main() {
  Map<String, String> countryCapital = {
    'USA': 'Washington, D.C.',
    'India': 'New Delhi',
    'China': 'Beijing'
  };

  // Loop Through For Each
  countryCapital.forEach((key,value)=> print('Key is $key and value is $value'));
}
```

**OUTPUT**
```
Key is USA and value is Washington, D.C.
Key is India and value is New Delhi
Key is China and value is Beijing
```