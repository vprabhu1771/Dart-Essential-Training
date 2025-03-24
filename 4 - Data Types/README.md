# 1 - List Data Types

Dart has a variety of built-in data types that you can use to declare variables and store different kinds of values. Here are the most commonly used data types in Dart:

1. Numbers:
   - `int`: Represents integer values, such as 1, 2, -5, etc.
   - `double`: Represents floating-point numbers, such as 3.14, -0.5, etc.

2. Strings:
   - `String`: Represents a sequence of characters, such as "Hello, Dart!" or 'OpenAI'.

3. Booleans:
   - `bool`: Represents boolean values, which can be either `true` or `false`.

4. Lists:
   - `List`: Represents an ordered collection of objects. It can contain elements of any type. Lists in Dart are zero-based, meaning the first element is at index 0.

5. Maps:
   - `Map`: Represents an unordered collection of key-value pairs. Keys and values can be of any type.

6. Sets:
   - `Set`: Represents an unordered collection of unique objects. Sets do not allow duplicate elements.

7. Runes:
   - `Runes`: Represents a sequence of Unicode code points. It is used for working with characters beyond the basic ASCII range.

8. Symbols:
   - `Symbol`: Represents an identifier that is unique within a Dart program. Symbols are often used for metaprogramming and reflection.

Additionally, Dart supports the concept of nullable types with the introduction of null safety in Dart 2.12 and later versions. This allows you to specify whether a variable can hold a null value or not by using the `?` modifier.

For example, you can declare a nullable integer variable like this: `int? nullableInt = null`.

These are the fundamental data types in Dart. You can also define your own custom data types using classes and enums to model more complex structures and behaviors in your code.

# 2 - Code Sample

Dart supports several data types, including:

1. Numbers: Dart has two main types for representing numbers:
   - `int`: Used for representing whole numbers (integers) without a fractional component. For example: `int age = 30;`
   - `double`: Used for representing numbers with a fractional component. For example: `double pi = 3.14;`

2. Strings: Dart represents strings of characters using the `String` type. Strings are enclosed in single quotes (`'`) or double quotes (`"`). For example: `String message = 'Hello, Dart!';`

3. Booleans: Dart has a Boolean type called `bool` that represents the values `true` or `false`. For example: `bool isRaining = true;`

4. Lists: Dart provides a built-in list type called `List` for representing ordered collections of objects. Lists can contain elements of different types. For example: 
   ```
   List<int> numbers = [1, 2, 3, 4, 5];
   List<String> names = ['Alice', 'Bob', 'Charlie'];
   ```

5. Maps: Dart has a map type called `Map` for representing key-value pairs. A map stores associations between keys and their corresponding values. For example:
   ```
   Map<String, int> scores = {
     'Alice': 90,
     'Bob': 85,
     'Charlie': 95,
   };
   ```

6. Sets: Dart provides a set type called `Set` for representing unordered collections of unique objects. Sets ensure that each element is unique and unordered. For example:
   ```
   Set<int> numbers = {1, 2, 3, 4, 5};
   Set<String> colors = {'red', 'green', 'blue'};
   ```

Here are some examples of using these data types:

```dart
int age = 30;
double pi = 3.14;

String message = 'Hello, Dart!';
bool isRaining = true;

List<int> numbers = [1, 2, 3, 4, 5];
List<String> names = ['Alice', 'Bob', 'Charlie'];

Map<String, int> scores = {
  'Alice': 90,
  'Bob': 85,
  'Charlie': 95,
};

Set<int> uniqueNumbers = {1, 2, 3, 4, 5};
Set<String> uniqueColors = {'red', 'green', 'blue'};
```

These examples demonstrate the basic usage of Dart's data types. Keep in mind that Dart also provides additional features and operations for working with these data types, such as methods, operators, and libraries that enhance their functionality.
