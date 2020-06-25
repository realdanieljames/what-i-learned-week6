# what-i-learned-week6

## Loops
### [definition](https://qhmit.com/javascript/tutorial/javascript_while_loop.cfm)
In JavaScript (and most other languages), "loops" enable your program to continuously execute a block of code for a given number of times, or while a given condition is true.  
***
### While Loops
while true, execute this   
syntax:
``` 
while(){}
while ('brackets'){'curlyBraces'}
while(['condition']){['code to execute while condition is true']}
```
The condition is evaluated before executing the statement.
*** 
### For Loops
#Designed for indices
if there is no "i" or "index" search. Use a while loop. 
*** 

## Arrays
[] 'square brackets'

**Add an item to an array**
```
variable[variables.length]
```
***

## Methods that were introduced to me in week 6

- **parseInt()**  
#The parseInt() method converts a string into an integer (a whole number). It accepts two arguments. ...  
***
- **parseFloat()**  
#The parseFloat() method converts a string into a point number (a number with decimal points). ...
***  

- **Number()**  
#The Number() method converts a string to a number.
https://gomakethings.com/converting-strings-to-numbers-with-vanilla-javascript/
***  

- **substring()**  
#The substring() method extracts the characters from a string, between two specified indices, and returns the new sub string.
This method extracts the characters in a string between "start" and "end", not including "end" itself.
***  
- **includes()**
#returns a boolean value(true/false)
***  
- **indexOf()**  
***  
- **typeof()**  
***  
- **pop()**  
#The pop() method removes the last element from an array:
#The pop() method returns the value that was "popped out":
```
let fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();              // Removes the last element ("Mango") from fruits
```  
***

- **push()**  
#The push() method adds a new element to an array (at the end):  
#The push() method returns the new array length:   


**push() Example**
```
Example
var fruits = ["Banana", "Orange", "Apple", "Mango"];
var x = fruits.push("Kiwi");   //  the value of x is 5
```
***

- **shift()**  
#Shifting is equivalent to popping, working on the first element instead of the last.  
The shift() method removes the first array element and "shifts" all other elements to a lower index.

**shift Example**
```
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();            // Removes the first element "Banana" from fruits
```
***  
- **slice()**  
#The slice() method returns a shallow copy of a portion of an array into a new array object.  
#selected from start to end (end not included) 
#start and end represent the index of items in that array.  
#The original array will not be modified.  

**syntax**
```
arr.slice([start[, end]])
```  

**slice Example**
```
let fruits = ['Banana', 'Orange', 'Lemon', 'Apple', 'Mango']
let citrus = fruits.slice(1, 3)

// fruits contains ['Banana', 'Orange', 'Lemon', 'Apple', 'Mango']
// citrus contains ['Orange','Lemon']
```
***

- **join()**  
#The join() method creates and returns a new string by concatenating all of the elements in an array (or an array-like object), separated by commas or a specified separator string. If the array has only one item, then that item will be returned without using the separator.  

**join() Example**
```
const elements = ['Fire', 'Air', 'Water'];

console.log(elements.join());
// expected output: "Fire,Air,Water"

console.log(elements.join(''));
// expected output: "FireAirWater"

console.log(elements.join('-'));
// expected output: "Fire-Air-Water"
```
***  

- **reverse()**  

The reverse() method reverses an array in place. The first array element becomes the last, and the last array element becomes the first.  

**syntax**
```
array.reverse() 
```
**reverse() Example**
```
const a = [1, 2, 3];

console.log(a); // [1, 2, 3]

a.reverse(); 

console.log(a); // [3, 2, 1]

```
***  

- **concat()**  
The concat() method is used to merge two or more arrays. This method does not change the existing arrays, but instead returns a new array.  

**concat() syntax**
```
const new_array = old_array.concat([value1[, value2[, ...[, valueN]]]])
```

**concat() Exapmle**
```
const array1 = ['a', 'b', 'c'];
const array2 = ['d', 'e', 'f'];
const array3 = array1.concat(array2);

console.log(array3);
// expected output: Array ["a", "b", "c", "d", "e", "f"]
```

cmd + D -- select all common words in vs code and edit it

- printing a variable with its output
result = 3 
console.log({result}) 
// result: 3
***
*** 

## tips and tricks

***string interpolation***

let num = 1;
while (num <= 5){
    console.log({num});
    num = num + 1;
}
console.log('done with loop');
console.log({num});
```