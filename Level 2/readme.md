1. Why do we use functions in JavaScript?
Ans. Functions in JavaScript are used to:
Encapsulate logic: Avoid code repetition by encapsulating a block of reusable code.
Organize code: Improve readability and maintainability by structuring code into smaller, logical units.
Modularize programs: Enable better debugging and testing by breaking a program into smaller pieces.
Allow dynamic behavior: Handle inputs and produce outputs dynamically.

2. What is Function Invocation?
Function invocation is the process of executing or calling a function. In JavaScript, this is done using parentheses ().
Examples:
function greet() {
    console.log("Hello, World!");
}
greet(); // Function invocation


3. Does a function behave like an object in JavaScript?
Yes, in JavaScript, functions are first-class objects. They can have properties and methods just like objects.


4. What are Events in JavaScript?
Events are actions or occurrences that happen in the browser, often initiated by user interaction or browser behavior. Examples include clicks, form submissions, mouse movements, or key presses.
Example of handling an event:
document.getElementById("myButton").addEventListener("click", function() {
    alert("Button clicked!");
});


5. What is a string?
A string is a sequence of characters used to represent text in JavaScript. Strings are enclosed in single quotes ('), double quotes ("), or backticks (`).

6. What is an array? Is it static or dynamic in JavaScript?
An array is a data structure used to store multiple values in a single variable. It is dynamic in JavaScript, meaning its size can change, and it can hold mixed data types.

7. What are array methods? List a few names.
Array methods are built-in functions that allow manipulation of arrays.
Examples:
push(): Adds elements to the end.
pop(): Removes the last element.
map(): Creates a new array by applying a function to each element.
filter(): Filters elements based on a condition.
reduce(): Reduces the array to a single value.
forEach(): Executes a function for each element in the array.
length: Returns the number of elements in the array.
indexOf(): Returns the index of the first occurrence of a value.
lastIndexOf(): Returns the index of the last occurrence of a value.

Projects

1. Reverse an array? Input: [1, 2, 3, 4, 5, 6]
const inputArray = [1, 2, 3, 4, 5, 6];
console.log(inputArray.reverse()); // Output: [6, 5, 4, 3, 2, 1]

2. Explain the properties of the join array method function via program?
function demonstrateJoinMethod() {
  const arr = ['Apple', 'Banana', 'Cherry', 'Date'];
  // Join the array with a comma (default separator)
  const result1 = arr.join();
  console.log("Joined with default separator (comma):", result1);
  // Join the array with a hyphen (-)
  const result2 = arr.join('-');
  console.log("Joined with hyphen (-):", result2);
  // Join the array with a space
  const result3 = arr.join(' ');
  console.log("Joined with space:", result3);
  // Join the array with no separator (empty string)
  const result4 = arr.join('');
  console.log("Joined with no separator:", result4);
  // Join an empty array
  const emptyArr = [];
  const result5 = emptyArr.join('-');
  console.log("Joined empty array:", result5); // Output: ''
}
demonstrateJoinMethod();

3. Show all the values of an array in a html webpage using DOM and forEach method?
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Display Array Values</title>
    <style>
        .array-item {
            font-size: 20px;
            margin: 5px;
        }
    </style>
</head>
<body>
    <h1>Array Values</h1>
    <div id="array-values"></div>
    <script>
        const myArray = [10, 20, 30, 40, 50];
        const container = document.getElementById('array-values');
        myArray.forEach(function(value) {
            const para = document.createElement('p');  // Create a new <p> element
            para.classList.add('array-item');  // Add a class for styling
            para.textContent = value;  // Set the text content of the <p> element to the array value
            container.appendChild(para);  // Append the <p> element to the container
        });
    </script>
</body>
</html>

4. Merge to sets in javascript? (hint use Set class in javascript)
const set1 = new Set([1, 2, 3]);
const set2 = new Set([3, 4, 5]);
const mergedSet = new Set([...set1, ...set2]);
console.log(mergedSet); // Output: Set {1, 2, 3, 4, 5}

