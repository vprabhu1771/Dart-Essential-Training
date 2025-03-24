# 1 - Standard Input

```
import 'dart:io';

void main() {
  stdout.write('Enter your name: ');
  String? name = stdin.readLineSync();

  stdout.write('Enter your age: ');
  int? age = int.parse(stdin.readLineSync()!);

  stdout.write('Enter your email: ');
  String? email = stdin.readLineSync();

  print('\n--- User Information ---');
  print('Name: $name');
  print('Age: $age');
  print('Email: $email');
}
```

**OUTPUT**
```
Enter your name: prabhu
Enter your age: 29
Enter your email: prabhu@gmail.com

--- User Information ---
Name: prabhu
Age: 29
Email: prabhu@gmail.com 
```

# 2 - Integer User Input

You can take integer input to get a numeric value from the user without the decimal point. E.g. 10, 100, -800 etc.

```
import 'dart:io';

void main() {
  print("Enter number:");
  int? number = int.parse(stdin.readLineSync()!);
  print("The entered number is ${number}");
}
```

**Output**
```
Enter number:
50
The entered number is 50
```

# 3 - Floating Point User Input

You can use float input if you want to get a numeric value from the user with the decimal point. E.g. 10.5, 100.5, -800.9 etc.

```
import 'dart:io';

void main() {
  print("Enter a floating number:");
  double number = double.parse(stdin.readLineSync()!);
  print("The entered num is $number");
}
```

**Output**
```
Enter a floating number:
55.5
The entered num is 55.5
```

# 4 - Character User Input

To create a program that allows user input for a character in Dart, you can use the 'stdin' object from the 'dart:io' library. Here's an example:

```
import 'dart:io';

void main() {

  stdout.write('Enter a Gender: ');

  String? input = stdin.readLineSync();

  if (input!.length > 0) 
  {
    
    var gender = input[0];

    print('Gender is $gender');

    var ascii = input.runes.first;

    print('Character ASCII: $ascii');

  } 
  else 
  {

    print('Invalid input. Please enter a single character.');

  }

}
```

**Output**
```
Enter a Gender: male
Gender is m
Character ASCII: 109

Enter a Gender: female
Gender is f
Character ASCII: 102
```

# 5 - String User Input

They are used for storing textual user input. If you want to keep values like somebody’s name, address, description, etc., you can take string input from the user.

```
import 'dart:io';

void main() {
  print("Enter name:");
  String? name  = stdin.readLineSync();
  print("The entered name is ${name}");
}
```

**Output**
```
Enter name:
prabhu

The entered name is prabhu
```