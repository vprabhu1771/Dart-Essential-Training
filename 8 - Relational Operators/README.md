# 1 - Relational Operators Table

| No | Relational Operators | Meaning                     |
|----|----------------------|----------------------------|
| 1  | <                   | Less Than                  |
| 2  | <=                  | Less Than or Equal to      |
| 3  | >                   | Greater Than               |
| 4  | >=                  | Greater Than or Equal to   |
| 5  | ==                  | Equal to                   |
| 6  | !=                  | Not Equal to               |

# 2 - Less Than Example

Perform comparison on both values

```
void main() {
    final int x = 1;
    
    final int y =  10;
    
    print(“x = $x”);
    
    print(“y = $y”);
    
    
    print(“$x < $y”);
    
    print(“${x < y}”);
}
```

**Output**
```
x = 1
y = 10
1 < 10
true
```

# 3 - Less Than or Equal To Example

Perform comparison on both values

```
void main() {
    final int x = 10;
    
    final int y =  10;
    
    print(“x = $x”);
    
    print(“y = $y”);
    
    
    print(“$x <= $y”);
    
    print(“${x <= y}”);
}
```

**Output**
```
x = 10
y = 10
10 <= 10
true
```

# 4 - Greater Than Example

Perform comparison on both values

```
void main() {
    final int x = 10;
    
    final int y =  1;
    
    print(“x = $x”);
    
    print(“y = $y”);
    
    
    print(“$x > $y”);
    
    print(“${x > y}”);
}
```

**Output**
```
x = 10
y = 1
10 > 1
true
```

# 5 - Greater Than or Equal To Example

Perform comparison on both values

```
void main() {
    final int x = 10;
    
    final int y =  10;
    
    print(“x = $x”);
    
    print(“y = $y”);
    
    
    print(“$x >= $y”);
    
    print(“${x >= y}”);
}
```

**Output**
```
x = 10
y = 10
10 >= 10
true
```

# 6 - Equal To Example

Perform comparison on both values

```
void main() {
    final int x = 10;
    
    final int y =  10;
    
    print(“x = $x”);
    
    print(“y = $y”);

    print(“$x == $y”);
    
    print(“${x == y}”);
}
```

**Output**
```
x = 10
y = 10
10 == 10
true
```

# 7 - Not Equal To Example

Perform comparison on both values

```
void main() {
    final int x = 20;
    
    final int y =  10;
    
    print(“x = $x”);
    
    print(“y = $y”);
    
    
    print(“$x != $y”);
    
    print(“${x != y}”);
}
```

**Output**
```
x = 20
y = 10
20 != 10
true
```