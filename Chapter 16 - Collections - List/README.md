# 1 - List

If you want to store multiple values in the same variable, you can use List. List in dart is similar to Arrays in other programming languages. E.g. to store the names of multiple students, you can use a List. The List is represented by Square Braces`[]`.

# 2 - How To Create List

You can create a List by specifying the initial elements in a square bracket. Square bracket `[]` is used to represent a List.

```
// Integer List
List<int> ages = [10, 30, 23];

// String List
List<String> names = ["Raj", "John", "Rocky"];

// Mixed List
var mixed = [10, "John", 18.8];
```

Types Of Lists

Fixed Length List
Growable List [Mostly Used]


# 3 - Fixed Length List

The fixed-length Lists are defined with the specified length. You cannot change the size at runtime. This will create List of 5 integers with the value 0.

```
void main() {  
   var list = List<int>.filled(5,0);  
   print(list);  
}
```

**OUTPUT**
```
[0, 0, 0, 0, 0]
```
Info

Note: You cannot add a new item to Fixed Length List, but you can change the values of List.

# 4 - Growable List

A List defined without a specified length is called Growable List. The length of the growable List can be changed in runtime.

```
void main() {  
   var list1 = [210,21,22,33,44,55];  
   print(list1);  
}  
```

**OUTPUT**
```
[210, 21, 22, 33, 44, 55]
```

# 5 - Access Item Of List

You can access the List item by index. Remember that the List index always starts with 0.

```
void main() {
  var list = [210, 21, 22, 33, 44, 55];

  print(list[0]);
  print(list[1]);
  print(list[2]);
  print(list[3]);
  print(list[4]);
  print(list[5]);
}
```

**OUTPUT**
```
210
21
22
33
44
55
```

# 6 - Get Index By Value

You can also get the index by value.

```
void main() {
  var list = [210, 21, 22, 33, 44, 55];

  print(list.indexOf(22));
  print(list.indexOf(33));
}
```

**OUTPUT**
```
2
3
```

# 7 - Find The Length Of The List

You can find the length of List by using .length property.

```
void main(){  
   List<String> names = ["Raj", "John", "Rocky"];
   print(names.length);
}
```

**OUTPUT**
```
3
```

Note: Remember that List index starts with 0 and length always starts with 1.

# 8 - Changing Values Of List

You can also change the value of List. You can do it by listName[index]=value;. For more, see the example below.

```
void main(){  
   List<String> names = ["Raj", "John", "Rocky"];
   names[1] = "Bill";
   names[2] = "Elon";
   print(names);
}
```

**OUTPUT**
```
[Raj, Bill, Elon]
```

# 9 - Mutable And Immutable List

A mutable List means they can change after the declaration, and an immutable List means they can’t change after the declaration.

```
List<String> names = ["Raj", "John", "Rocky"]; // Mutable List
names[1] = "Bill"; // possible
names[2] = "Elon"; // possible
    
const List<String> names = ["Raj", "John", "Rocky"]; // Immutable List
names[1] = "Bill"; // not possible
names[2] = "Elon"; // not possible
```

# 10 - first

It returns the first element in the List.

```
void main() 
{
   
   List<String> drinks = ["water", "juice", "milk", "coke"];
   
   print("First element of the List is: ${drinks.first}");
   
}
``` 

**OUTPUT**
```
First element of the List is: water
```

# 11 - last

It returns the last element in the List.

```
void main() 
{
   
   List<String> drinks = ["water", "juice", "milk", "coke"];
   
   print("Last element of the List is: ${drinks.last}");
   
}   
```

**OUTPUT**
```
Last element of the List is: coke
```

# 12 - isEmpty

It returns true if the List is empty and false if the List is not empty.

```
void main() 
{
  List<String> drinks = ["water", "juice", "milk", "coke"];
   
  List<int>  ages = [];
   
  print("Is drinks Empty: "+drinks.isEmpty.toString());
   
  print("Is ages Empty: "+ages.isEmpty.toString());
   
}
```

**OUTPUT**
```
Is drinks Empty: false
Is ages Empty: true
```

# 13 - isNotEmpty

It returns true if the List is not empty and false if the List is empty.

```
void main() 
{
  List<String> drinks = ["water", "juice", "milk", "coke"];
   
  List<int>  ages = [];
   
  
  print("Is drinks not Empty: "+drinks.isNotEmpty.toString());
  
  print("Is ages not Empty: "+ages.isNotEmpty.toString());
   
}  
```

**OUTPUT**
```
Is drinks not Empty: true
Is ages not Empty: false
```

# 14 - length

It returns the length of the List.

```
void main() 
{
  List<String> drinks = ["water", "juice", "milk", "coke"];  
  
  print("Length is : "+drinks.length.toString());
   
}
```

**OUTPUT**
```
Length is : 4
```

# 15 - reversed

It returns a List in reverse order.

```
void main() 
{
  List<String> drinks = ["water", "juice", "milk", "coke"];  
  
  print("List in reverse: ${drinks.reversed}");
   
}  
```

**OUTPUT**
```
List in reverse: (coke, milk, juice, water)
```

# 16 - single

It is used to check if the List has only one element and returns it.

```
void main() 
{

  List<String> drinks = ["water"];  
  
  print("is Single Element: ${drinks.single}");
   
}  
```

**OUTPUT**
```
water
```

# 17 - add

Add one element at a time and returns the modified List object.

```
void main() 
{  
    var evenList = [2,4,6,8,10];

    print(evenList); 

    evenList.add(12);

    print(evenList);      
}  
```

**OUTPUT**
```
[2, 4, 6, 8, 10]
[2, 4, 6, 8, 10, 12]
```

# 18 - addAll

Insert the multiple values to the given List, and each value is separated by the commas and enclosed with a square bracket ([]).

```
void main() 
{
  var evenList = [2, 4, 6, 8, 10];

  print(evenList);

  evenList.addAll([12, 14, 16, 18]);

  print(evenList);  
}
```

**OUTPUT**
```
[2, 4, 6, 8, 10]
[2, 4, 6, 8, 10, 12, 14, 16, 18]
```

# 19 - insert

Provides the facility to insert an element at a specified index position.

```
void main() {

  List myList = [3, 4, 2, 5];

  print(myList);

  myList.insert(2, 15);

  print(myList);

}
```

**OUTPUT**
```
[3, 4, 2, 5]
[3, 4, 15, 2, 5]
```

# 20 - InsertAll

Insert the multiple value at the specified index position.

```
void main() {
  var myList = [3, 4, 2, 5];

  print(myList);

  myList.insertAll(1, [6, 7, 10, 9]);

  print(myList);
}
```

**OUTPUT**
```
[3, 4, 2, 5]
[3, 6, 7, 10, 9, 4, 2, 5]
```

# 21 - replaceRange

The replaceRange method allows you to replace a range of elements or characters within the string or list with new elements or characters.

Here's the general syntax for using replaceRange:

String replaceRange(int start, int end, String replacement)
List<E> replaceRange(int start, int end, Iterable<E> replacement)

start: The index at which to start replacing elements or characters.

end: The index just after the end index of the range to be replaced. This means that the element or character at this index will not be included in the replacement.

replacement: The new string or list of elements that will replace the specified range.

```
void main() {
  var list = [10, 15, 20, 25, 30];

  print("List before updation: ${list}");

  list.replaceRange(0, 4, [5, 6, 7, 8]);

  print("List after updation using replaceAll() function : ${list}");
}
```

**OUTPUT**
```
List before updation: [10, 15, 20, 25, 30]
List after updation using replaceAll() function : [5, 6, 7, 8, 30]
```

# 22 - remove

In this example below, we are removing item of List using remove() method.

```
void main() {

  var list = [10, 20, 30, 40, 50];

  print("List before removing element : ${list}");

  list.remove(30);

  print("List after removing element : ${list}");

}
```

**OUTPUT**
```
List before removing element : [10, 20, 30, 40, 50]
List after removing element : [10, 20, 40, 50]
```

# 23 - removeAt

In this example below, we are removing item of List using removeAt() method.

```
void main() {

  var list = [10, 11, 12, 13, 14];

  print("List before removing element : ${list}");

  list.removeAt(3);

  print("List after removing element : ${list}");

}
```

**OUTPUT**
```
List before removing element : [10, 11, 12, 13, 14]
List after removing element : [10, 11, 12, 14]
```

# 24 - removeLast

In this example below, we are removing last item of List using removeLast() method.

```
void main() {

  var list = [10, 20, 30, 40, 50];

  print("List before removing element:${list}");

  list.removeLast();

  print("List after removing last element:${list}");

}
```

**OUTPUT**
```
List before removing element:[10, 20, 30, 40, 50]
List after removing last element:[10, 20, 30, 40]
```

# 25 - removeRange

In this example below, we are removing the range of items of List using removeRange() method.

```
void main() {

  var list = [10, 20, 30, 40, 50];

  print("List before removing element:${list}");

  list.removeRange(0, 3);

  print("List after removing range element:${list}");

}
```

**OUTPUT**
```
List before removing element:[10, 20, 30, 40, 50]
List after removing range element:[40, 50]
```

# 26 - forEach

You can use for loop, for each loop, or any other type of loop.

```
void main() {

  List<int> list = [10, 20, 30, 40, 50];

  list.forEach((n) => print(n));

}
```

**OUTPUT**
```
10
20
30
40
50
```

# 27 - map

This example below multiply value of List item by 2.

```
void main() {

  List<int> list = [10, 20, 30, 40, 50];

  var douledList = list.map((n) => n * 2);

  print((douledList));

}
```

**OUTPUT**
```
(20, 40, 60, 80, 100)
```

# 28 - spread

You can combine two or more Lists in dart by using spread syntax.

```
void main() {

  List<String> names = ["Raj", "John", "Rocky"];

  List<String> names2 = ["Mike", "Subash", "Mark"];

  List<String> allNames = [...names, ...names2];

  print(allNames);

}
```

**OUTPUT**
```
[Raj, John, Rocky, Mike, Subash, Mark]
```

# 29 - Conditions

You can also use conditions in List. Here sad = false so cart doesn’t contain Beer in it.

```
void main() {
  bool sad = false;

  var cart = ['milk', 'ghee', if (sad) 'Beer'];

  print(cart);
}
``` 

**OUTPUT**
```
[milk, ghee]
```

# 30 - where

You can use where with List to filter specific items. Here in this example, even numbers are only filtered.

```
void main(){
  List<int> numbers = [2,4,6,8,10,11,12,13,14];

  List<int> even = numbers.where((number)=> number.isEven).toList(); 

  print(even);
}
```

**OUTPUT**
```
[2, 4, 6, 8, 10, 12, 14]
```