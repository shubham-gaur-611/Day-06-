1. What is JavaScript?
Ans. JavaScript is a high-level, interpreted programming language widely used for creating interactive and dynamic content on web pages. It is one of the core technologies of the World Wide Web, alongside HTML and CSS.

2. What is the difference between b/w let and var?
Ans. The main differences between let and var in JavaScript lie in scope, hoisting, redeclaration, and block-level behavior.

3. Why do we prefer const over var?
Ans. We prefer const over var in modern JavaScript for better code stability, predictability, and maintainability. 

4. What is the use of javascript in web browsers?
Ans. JavaScript enables web pages to respond to user interactions without requiring a page reload.
     JavaScript allows developers to interact with the Document Object Model (DOM) to dynamically update the structure, style, and content of a web page.

5. What are Objects?
Ans. In JavaScript, objects are collections of related data and functionality organized as key-value pairs. They are one of the fundamental data types and allow developers to store, retrieve, and manipulate complex data structures.

6. What is an array and how is it different from an Object in Javascript?
Ans. An array is an ordered collection of elements, where each element is identified by a numerical index, starting from zero. Arrays are ideal for storing lists of items where the order is significant.

7. What is a function?
Ans. In JavaScript, a function is a block of reusable code designed to perform a specific task. Functions take input (optional), process it, and return an output (optional). They are fundamental building blocks for creating modular, organized, and reusable code.

8. How can we implement call by value and call by reference in Javascript?
Ans. Call by Value
Definition:
A copy of the actual value is passed to the function.
Changes made to the parameter inside the function do not affect the original value.
Applies to: Primitive types (e.g., number, string, boolean, null, undefined, symbol, bigint).

Call by Reference
Definition:
A reference to the actual memory location is passed to the function.
Changes made to the parameter inside the function do affect the original value.
Applies to: Non-primitive types (e.g., objects, arrays).

9. What are the primitive data types in Javascript?
Ans. In JavaScript, primitive data types are the most basic types of data. They are immutable (cannot be altered) and are passed by value.
     Primitive types (e.g., number, string, boolean, null, undefined, symbol, bigint).

10. What is DOM?
Ans. The DOM (Document Object Model) is a programming interface provided by web browsers that allows developers to interact with and manipulate the structure, content, and style of a web document dynamically.

11. Why do we need DOM?
Ans. The DOM provides a way to access and manipulate the structure, content, and style of a web document, enabling developers to create interactive and dynamic web pages.


Projects:

1. Average of array nums in Javascript?
const nums = [1, 2, 3, 4, 5];
let sum = 0;
nums.forEach((num) => {
    sum += num;
})
console.log(sum/nums.length);

2. Swap two numbers by reference?
function swapNumbers(obj) {
  const temp = obj.num1;
  obj.num1 = obj.num2;
  obj.num2 = temp;
}
const numbers = { num1: 5, num2: 10 };
console.log("Before swap:", numbers);
swapNumbers(numbers);
console.log("After swap:", numbers); 

3. Print the fibonacci sequence?
function printFibonacci(n) {
  let a = 0, b = 1;
  console.log(a);
  if (n > 1) {
    console.log(b);
  }
  for (let i = 2; i < n; i++) {
    const next = a + b;
    console.log(next);
    a = b;
    b = next;
  }
}
const n = 10;
printFibonacci(n);

4. Sort an array by both ascending and descending order?
function sortArray(arr) {
  const sortedAsc = arr.slice().sort((a, b) => a - b);
  const sortedDesc = arr.slice().sort((a, b) => b - a);
  return [sortedAsc, sortedDesc];
}
const arr = [5, 2, 8, 3, 1, 9];
console.log(sortArray(arr));

5. Show a variable value in an HTML webpage using DOM?
const element = document.getElementById("myElement");
element.innerHTML = "Hello, World!";

