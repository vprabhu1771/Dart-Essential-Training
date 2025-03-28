# 1 - User Defined Functions

In Dart, you can define your own functions to encapsulate reusable blocks of code. Functions allow you to organize your code, make it more readable, and avoid duplicating code. Here's how you can define user-defined functions in Dart:

Syntax of a function declaration:

```dart
returnType functionName(parameters) {
  // Function body
  // Code to be executed
  return value; // Optional return statement
}
```

Explanation of each component:

- `returnType`: The data type of the value returned by the function. Use `void` if the function doesn't return any value.
- `functionName`: The name of the function, which should be a descriptive and meaningful identifier.
- `parameters`: The inputs that the function receives. Parameters are optional, and you can define zero or more parameters. Each parameter consists of a data type followed by its name.
- `Function body`: The block of code that contains the statements to be executed when the function is called.
- `return` statement: If the function has a return type other than `void`, you can use the `return` statement to return a value from the function. It terminates the function execution and passes the value back to the caller.

Examples:

1. Function without parameters and return type:
   ```dart
   void greet() {
     print('Hello, Dart!');
   }
   ```
   In this example, the `greet` function doesn't take any parameters and doesn't return any value. It simply prints "Hello, Dart!" when called.

2. Function with parameters and return type:
   ```dart
   int addNumbers(int a, int b) {
     return a + b;
   }
   ```
   This example defines a function named `addNumbers` that takes two parameters (`a` and `b`) of type `int`. It calculates the sum of `a` and `b` and returns the result.

3. Function with optional parameters:
   ```dart
   void printFullName(String firstName, {String lastName = ''}) {
     print('Full Name: $firstName $lastName');
   }
   ```
   Here, the `printFullName` function has one required parameter (`firstName`) and one optional parameter (`lastName`). The optional parameter is enclosed in curly braces `{}` and has a default value of an empty string. The function can be called with or without providing a value for `lastName`.

Calling functions:

To call a function, you use the function name followed by parentheses `()`. If the function has parameters, you provide the corresponding values inside the parentheses.

Examples:

```dart
greet(); // Calling the greet() function

int sum = addNumbers(3, 5); // Calling the addNumbers() function and storing the result in the sum variable

printFullName('John'); // Calling the printFullName() function with only the required parameter

printFullName('Jane', lastName: 'Doe'); // Calling the printFullName() function with both parameters
```

These are some basic examples of defining and calling user-defined functions in Dart. Functions are a powerful feature of Dart that allow you to organize and reuse code effectively.