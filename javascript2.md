# Javascript Part II

1. You can use javascript to select any element, attribute, or text from an HTML page.
2. You can use javascript to add elements, attributes, and text to the page, or remove them.
3. You can make a set of steps for the browser to follow which allows it to access or change the content of a page.
4. You can specify that a script should run when a specific event has occurred.

A **script** is a series of instructions. You can compare scripts to recipes, handbooks, or manuals. To write one, you need to first _state your goal_ and then list the tasks that need to be completed in order to achieve it. To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help).

An **expression** results into a single value. There are generally two types of expressions:
1. Expressions that just assign a value to a variable.
```javascript
var color = 'beige';
//The value of the color is now beige.
```
2. Expressions that use two or more values to return a single value.
```javascript
var area = 3 * 2;
//The value of area is now 6.
```
Expressions rely on things called **operators**.

1. Assignment Operators
    - assign a value to a variable
    ```javascript
    color = 'beige';
    ```
2. Arithmetic Operators
    - perform basic math
    ```javascript
    area = 3 * 2;
    ```
3. String Operators
    - combine two strings
    ```javascript
    greeting = 'Hi ' + 'Molly';
4. Comparison Operators
    - compare two values and return true or false
    ```javascript
    buy = 3 > 5;
5. Logical Operators
    - combine expressions and return true or false
    ```javascript
    buy = (5 > 3) && (2 < 4);
    ```
To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is **function declaration**.