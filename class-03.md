## Lists & Boxes

### Lists

There are three types of lists:
1. **Ordered** Lists - `<ol>`
  - use numbers
  - each item in the list is placed between an opening and closing `<li>` tag.
2. **Unordered** Lists
  - use bullets
  - each item in the list is placed between an opening and closing `<li>` tag.
3. **Definition** Lists - `<dl>`
  - used to define terminology.
  - `<dt>` is used to contain the term being defined.
  - `<dd>` is used to contain the definition.

  - You can also put a second list inside an `<li>` element to create a sub list (nested list).

### Boxes

By default, boxes around text are only big enough to hold whats inside. You can set your own dimensions with the **height** and **width** properties.
```css
div {
  height: 300px;
  width: 300px;
}
p {
  height: 75%;
  width: 75%;
}
```
- you can use pixels or percentages
- every box has three available properties that can be adjusted to control the appearance.
1. Border - separates the edge of one box from another
2. Margin - sits outside the edge of the border
3. Padding - the space between the border of a box and any content inside
- if you want to center a box on the page (or center it inside the element its it), you can use `text-align: center;`
- The _padding_ and _margin_ properties are very helpful in adding space between various items.
- use `display: inline;` on list items to make them flow horizontally.
    - block level boxes can be made into inline boxes, and inline boxes made into block level boxes.

### Arrays

An **array** is a variable that stores a list of _values_. You should consider using an array when you have a list or set of values that are related to each other.
- arrays are created by giving it a name as you would any other variable.
- seperate values with commas
```javascript
var colors;
colors = ['white', 'black', 'custom'];

var el = document.getElementById('colors');
el.textContent = colors[0];
```
Above is an array created by using the array literal technique.
```javascript
var colors = new Array('white', 
                        'black',
                        'custom');

var el = document.getElementById('colors');
el.innerHTML = colors.item(0);
```
Above is an array created using the array constructor technique.
Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of it starts at zero (not one). Each item in an array is automatically given a number called the **index**.

### If Else Statements

The `if else` statement checks a condition. If it resolves to true, the first code block `if` is executed. If the condition is false, the second code block `else` is executed.

### Switch Statements

A **switch** statement starts with a variable called the switch value. Each **case** indicates a possible value for this variable and the code that should run if the variable matches taht value.
```javascript
switch (level) {

  case 'One':
  title = 'Level 1';
  break;

  case 'Two':
  title = 'Level 2';
  break;

  case 'Three':
  title = 'Level 3';
  break;

  default:
  title= 'Test';
  break;
}
```
_Level_ is the switch value.

### Loops

Loops check a condition. If it returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. This process is repeated until the condition returns false.

- For Loops
  - used for running code a specific number of times.
- While Loops
  - used for if you don't know how many times the code should run.
- Do While Loops
  - similar to the while, but always runs the statements inside the curly braces at least once, even if the condition evaluates to false.
```javascript
for (var i = 0; i < 10; i++) {
  document.write(i);
}
```
This is a for loop.
Conditions are made up of three statements:
- Initialization
  `var i = 0;`
  - the variable is only created the first time.
- Condition
  `i < 10;`
  - the value of i was initially set to 0, so in this case the loop will run 10 times before stopping.
- Update
  `i++`
  - one is added to the counter.

**Continue** this keyword tells the interpreter to continue with the current iteration.

**Break** this keyword causes the termination of a loop and tells the interpreter to go onto the next statement of code outside of the loop.

[<===Home](README.md)