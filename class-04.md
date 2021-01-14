# Links and Layout

## Writing Links

Links are created using the `<a>` element. Users can click on anything between the opening `<a>` tag and the closing tag. Using the _href_ attribute, you can specify which page you want to link.

```html
<a href="http://www.imdb.com">IMDB </a>
```
**If all the pages of the site are in the same folder, then the value of href can just be the name of the file.**

Here are some relative link types:
1. Child Folder
  - use the name of the child folder, followed by a forward slash, then the file name.
2. Grandchild Folder
  - use the name of the child folder, followed by a forward slash, then the name of the grandchild foler, followed by another forward slash, then the file name.
3. Parent Folder
  - use ../ to indicate the folder above the current one, then follow it with the file name.
4. Grandparent Folder
  - repeat the ../ to indicate that you want to go up two folders, then folow it with the file name.

- Email Link
To create a link that starts up the user's **email** program and addresses an email to a specified email address, use the `<a>` element. This time, the value of the href attribute starts with **mailto:** and is followed by the email address.
- Target
If you want a link to open in a new window, you can use the target attribute on the opening `<a>` tag. Example: `<a href="http://www.imdb.com" target="_blank">`

## Layout

#### Key Concepts in Positioning Elements

CSS treats each HTML element as if it's in it's own box. This box will eitlher be a **block-level** or an **inline** box.

- block-level boxes start on a new line and act as the main building blocks of any layout. Ex: `<h1>` `<p>`
- inline boxes flow between surrounding text. Ex: `<img>`
- to indicate where a box should be positioned, you may also need to use **box offset** properties to tell the browser how far from the top or bottom and left or right it should be placed.
- the **float** property moves content to the left or right of the page and can be used to create multi-column layouts.

If one block-level element sits inside another, then the outer box is known as the **containing** or **parent** element. It is common to group a number of elements together inside a `<div>` element.

CSS has the following positioning schemes that allow you to control the layout of a page:
1. Normal Flow
  - every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.
2. Relative Positioning
  - this moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.
3. Absolute Positioning
  - this positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements.
4. Fixed Positioning
  - this is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element.
5. Floating Elements
  - floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box.

- Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens. 
- Because screen sizes and dislplay resolutions vary so much, web designers often try to create pages of around **960-1000** pixels wide.
- **fixed width layout** designs do not change size as the user increases or decreases the size of their browser or window.
- **liquid layout** designs stretch and contact as the user increases or decreases the size of their browser window.
- Grids help create good designs
- You can include multiple CSS files in one page.

# Functions, Methods & Objects

1. Functions
  - functions let you group a series of statements together to perform a specific task. Allows you to reuse code without having to repeat the same set of statements over and over again.
```javascript
var msg = 'Sign up to receive our newsletter for 10% off!';
function updateMessage() {
  var el = document.getElementById('message');
  el.textContent = msg;
}
updateMessage();
```
To create a funtion, you give it a name and then write the statements needed to achieve its task inside the curly braces. Above, we declared `updateMessage()` a function. To call the function you simply type it out, followed by a semicolon.
- sometimes when you declare the function you give it **parameters**. Inside the function, the parameters act like variables.
- when you call a function that has parameters, you specify the values it should use in the parentheses that follow its name.
```javascript
funtion calculateArea(width, height) {
  var area = width * height;
  return area;
}
var wallOne = calculateArea(3, 5);
var wallTwo = calculateArea(8, 5);
```
- This `calculateArea()` function returns the area of a rectangle to the code that called it.
- inside the function, a variable called **area** is created. It holds the calculated area of the box. The **return** keyword is used to return a value to the code that called the function.

Functions can return more than one value using an array.
```javascript
function getSize(width, height, depth) {
  var area = width * height;
  var volume = width * height * dpeth;
  var sizes = [area, volume];
  return sizes;
}
var areaOne = getSize(3, 2, 3)[0];
var volumeOne = getSize(3, 2, 3)[1];
```
- a new function is created called `getSize()`
- the area of the box is calculated and stored in a variable called area
- the volume is calculated and stored in a variable called volume
- this array is then returned to the code that called the `getSize()` function, allowing the values to be used.
- the `areaOne` variable holds the area of a box that is 3 * 2. This is the first value in the **sizes** array.
- the `volumeOne` variable holds the volume of a box that is 3 * 2 * 3. This is the second value in the **sizes** array.

### Pair Programming

Pair programming often involves two roles: the driver and the navigator. The **driver** is the programmer who is typing and the only one whose hands are on the keyboard. The **navigator** guides the driver using their words. The navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs.

#### Why pair program?

1. Greater efficiency
  - research indicates that pair programming takes slightly longer, but produces higher quality code.
2. Engaged collaboration
  - it is harder to procrastinate or get off track when someone else is relying on you to complete the work.
3. Learning from fellow students
  - everyone has a different way to doing things, working with a teammate can expose developers to techniques they otherwise would not have thought of.
4. Social skills
  - pair programming is great for improving social skills
5. Job interview readiness
  - a common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen.
6. Work environment readiness
  - many companies that utilize pair programming expect to train fresh hires. If you're already familiar with how pairing works, you can hit the ground running at a new job.

  [<===Home](README.md)