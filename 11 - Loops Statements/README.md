# 1 - for loop

for loop:
The for loop is used to iterate a specific number of times. It consists of three parts: initialization, condition, and increment/decrement.

```
for (initialization; condition; increment/decrement) {
  // Code to be executed
}
```

```
for (var i = 0; i < 5; i++) {
  print('Iteration $i');
}
```

**Output**
```
Iteration 0
Iteration 1
Iteration 2
Iteration 3
Iteration 4
```

# 2 - while loop

The while loop repeatedly executes a block of code as long as a given condition is true.

```
while (condition) {
  // Code to be executed
}
```

```
var count = 0;

while (count < 5) {
  print('Count: $count');
  count++;
}
```

**Output**
```
Count: 0
Count: 1
Count: 2
Count: 3
Count: 4
```

# 3 - do-while loop

The do-while loop is similar to the while loop, but it checks the condition after executing the block of code. Therefore, the code inside the loop will always run at least once.

```
do {
  // Code to be executed
} while (condition);
```

```
var i = 0;

do {

  print('Iteration $i');
  
  i++;

} while (i < 5);
```

**Output**
```
Iteration 0
Iteration 1
Iteration 2
Iteration 3
Iteration 4
```