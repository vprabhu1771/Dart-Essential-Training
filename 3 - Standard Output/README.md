# Dart Basics

## 1 - Print Statement

```dart
void main()
{
  print('Hello, World!');
}
```

**Output:**
```
Hello, World!
```

## 2 - Using stdout for Input

```dart
import 'dart:io';

void main()
{
  // The text will be displayed without a newline character.
  stdout.write('Enter your name: ');
  
  // Read user input from stdin.
  var name = stdin.readLineSync();

  print('Hello, $name!');
}
```

**Output:**
```
Enter your name: prabhu
Hello, prabhu!
```

## 3 - String Concatenation - Using the '+' Operator

```dart
void main() {
  String str1 = "Hello";
  String str2 = "World";
  String result = str1 + " " + str2;
  print(result);
}
```

**Output:**
```
Hello World
```

## 4 - String Concatenation - Using String Interpolation

```dart
void main() {
  String str1 = "Hello";
  String str2 = "World";
  String result = "$str1 $str2";
  print(result);
}
```

**Output:**
```
Hello World
```
