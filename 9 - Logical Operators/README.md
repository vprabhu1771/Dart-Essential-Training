# 1 - Logical Operators Table

No	Logical Operators	Meaning
1	&&	AND 
2	||	OR

# 2 - AND Example

Perform comparison on both Logical Test

```
void main() {
    final int x = 1;
    
    final int y =  10;
    
    print(“x = $x”);
    
    print(“y = $y”);
    
    
    print(“$x < $y && $x != $y”);
    
    print(“${x < y && x != y}”);
}
```

**Output**
```
x = 1
y = 10
1 < 10 && 1 != 10
true
```

# 3 - OR Example

Perform comparison on both Logical Test

```
void main() {
    final int x = 1;
    
    final int y =  10;
    
    print(“x = $x”);
    
    print(“y = $y”);
    
    
    print(“$x > $y || $x != $y”);
    
    print(“${x > y || x != y}”);
}
```

**Output**
```
x = 1
y = 10
1 > 10 || 1 != 10
true
```