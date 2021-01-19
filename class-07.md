## Domain Modeling
- domain modeling is the process of making a model in code for a specific problem.
- Here's an implementation of a constructor function:
```javascript
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```
- here's an example of a random number generator:
```javascript
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail.generateRandom(1, 5));
console.log(corgiFail.generateRandom(1, 5));
```
- methods can be added to a constructor function.
## Tables
- `<table>` is used to create a table.
  - `<tr>` is used to indicate the start of each row. At the end of each row you use a closing tag.
  - `<td>` each cell of the table is represented using this. Use a closing tag to end the cell.
- `<th>` is used just like the `<td>` element but its used to represent the heading for either a column or a row.
  - the `colspan` attribute can be used on a `<th>` or `<td>` element and indicates how many columns that cell should run across.
## Creating an Object
- the **new** keyword and the object constructor create a blank object. You can then add properties and methods to the object.
```javascript
var hotel = new Object();

hotel.name = 'Quay';
hotel.rooms = 40;
hotel.booked = 25;
hotel.checkAvailability = function()  {
  return this.rooms - this.booked;
};
```
- you can use this syntax to add properties and methods to any object you have created.
- to update the value of properties, use dot notation or square braackets. `hotel.name = 'Park';`
  - if the object does not have the property you are trying to update, it will be added.
- sometimes you will want several objects to represent similar things. **Object constructors** can use a function as a template for creating objects.
```javascript
function Hotel(name, rooms, booked) {
  this.name = name;
  this.rooms = rooms;
  this.booked = booked;
  this.checkAvailability = function() {
    return this.rooms - this.booked;
  };
}
```
- you create instances of the object using the constructor function.
- the **new** keyword followed by a call to the function creates a new object. For example:
```javascript
var quayHotel = new Hotel('Quay', 40, 25);
var parkHotel = new Hotel('Park', 120, 77);
```
- ways to create objects - **pg. 113**
- the keyword `this` is commonly used inside functions and objects. Where the function is declared alters what `this` means. It always refers to one object, usually the object in which the function operates.
- when a function is created at the top level of a script(unless it is inside another function) it is in the **global script** or **global context**.
- objects are like **arrays** except instead of index numbers, **objects** have property names.
- you can combine arrays and objects to create complex data structures.
- **arrays** can store a series of objects and remember their order
- **objects** can hold arrays as values of their properties

Arrays in an object
```javascript
//The rooms are the properties, items are the values.
room1 = items[420, 40, 10]
room2 = items[460, 20, 20]
room3 = items[230, 0, 0]
room4 = items[620, 150, 60]
```
To access the first charge for room1 you would use `costs.room1.items[0];`

Objects in an Array
```javascript
//First numbers are the index numbers.
0 = {accom: 420, food: 40, phone: 10}
1 = {accom: 460, food: 20, phone: 20}
2 = {accom: 230, food: 0, phone: 0}
3 = {accom: 620, food: 150, phone: 60}
```
To access the phone charge for room three, you would use `costs[2].phone;`

### Three Groups of Built-In Objects
1. Browser object model
  - creates a model of the browser tab or window.
  - example: the window object's `print()` method will cause the browser's print dialog box to be shown: `window.print();`
2. Document Object Model
  - creates a model of the current web page. The top most object is the **document** object, which represents the page as a whole. It's child object represent other items on the page.
  - example: the document object's `getElementById()` method gets an element by the value of its id attribute: `document.getElementById('one');`
3. Global Javascript Objects
  - these do not form a single model. They are a group of individual objects that relate to different parts of the javascript language.
  - the names of the global objects usually start with a capital letter. Example: the string object's toUpperCase() method makes all letters in the following variable uppercase: `hotel.toUpperCase();`.
- in order to work with dates, you create an instance of the **date** object.
- `var today = new Date();` - think of this as creating a variable called **today** that holds a number. In javascript, dates are stored as a number: specifically the number of milliseconds since midnight on january 1, 1970.
- functions allow you to group a set of related statements together that represent a single task. 
- functions can take parameters (information required
to do their job) and may return a value. 

[<===Home](README.md)