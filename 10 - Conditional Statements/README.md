# 1 - Conditions Statements Topics

1. **if statement**  
2. **if else statement**  
3. **if else with logical operator**  
4. **nested if else statement**  
5. **nested if else statement with logical operators**  
6. **if expression** (similar to ternary operator)  
7. **when statement** (similar to switch statement)  

# 2 - if statement

```
void main() {
    final int age = 18;
    
    if (age >= 18)
    {
        print("Congrats. You are Eligible for voting");
    }
}
```

**Output**
```
Congrats. You are Eligible for voting
```

# 3 - if else statement

```
void main() {
    
    final int age = 18;
    
    if (age >= 18)
    {
    	print("Congrats. You are eligible for voting");  
    }
    else
    {
        print("Sorry. You are not eligible for voting");
    }
    
}
```

**Output**
```
Congrats. You are eligible for voting
```

# 4 - if else with logical operator

```
void main() {
    
    final int age = 100;
    
    if (age >= 18 && age <= 100)
    {
    	print("Congrats. You are eligible for voting");
    }
    else
    {
        print("Sorry. You are not eligible for voting");
    }
    
}
```

**Output**
```
Congrats. You are eligible for voting
```

# 5 - nested if else statements

```
void main() {
    
    final int age = 20;
    
    if (age >= 18)
    {
    	print("your age is over 18");
        
        if (age >= 20)
        {
            print("your age is over 20");
        }
        else
        {
            print("your age below 20");
        }
    }
    else
    {
        print("your age is over 18");
    }
    
}
```

**Output**
```
your age is over 18
your age is over 20
```

# 6 - nested if else statement with logical operators

```
void main() {
    
    final int age = 20;
    
    if (age >= 18 && age <= 22)
    {
    	print("Congrats. You are eligible for Home Loan");
        
        if (age >= 18 && age <= 20)
        {
            print("Car loan also available");
        }
        else
        {
            print("Car loan not available");
        }
    }
    else
    {
        print("Sorry. You are not eligible for Home Loan");
    }
    
}
```

**Output**
```
Congrats. You are eligible for Home Loan
Car loan also available
```

# 7 - If alternative - Ternary Operator

```
void main() {

  final int age = 20;

  print(age >= 18 ? "eligible for voting" : "not eligible for voting");

}
```

**Output**
```
eligible for voting
```

# 8 - Switch Statement

```
void main() {

  int option = 1;

  switch (option) {
    case 1:
      print('Good Morning');
      break;
    case 2:
      print('Good Afternoon');
      break;
    case 3:
      print('Good Evening');
      break;
    case 4:
      print('Good Night');
      break;
    default:
      print('Invalid Options');
  }

}
```

**Output**
```
Good Morning
```