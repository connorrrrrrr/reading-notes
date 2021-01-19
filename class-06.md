## What is an Object?

**Objects** group together a set of variables and functions to create a model of something you would recognize from the real world. In an **object**, variables become known as properties and functions become known as **methods**.

```javascript
var hotel = {

  name: 'Quay', //These are properties
  rooms: 40,    //--------------------
  booked: 25,   //--------------------
  gym: true,    //--------------------
  roomTypes: ['twin', 'double', 'suite'], //---------------

  checkAvailability: function() {   //This is a function
    return this.rooms - this.booked;//------------------
  } //--------------------------------------------------
};
```
- **Literal notation** is the easiest and most popular way to create objects. In the example above, the **object** is stored in a variable called _hotel_.
- to access a property or method of an object you use the name of the object, followed by a period, then the name of the property or method. This is known as **dot notation**. 
```javascript
var hotelName = hotel.name;
var roomsFree = hotel.checkAvailability();
```
- you can also access the properties of an object (but not it's methods) using square bracket syntax. `var hotelName = hotel['name'];`

# Document Object Model

- the document object model (dom) specifies how browsers should create a model of an HTML page and how Javascript can access and update the contents of a web page while it is in the browser window.
- accessing and uploading the dom tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.
- methods that find elements in the dom tree are called **dom queries**.
- when people talk about storing elements in variables, they are really storing the location of the elements within the dom tree in a variable.

### Methods That Return a Single Element Node
- `getElementById` selects an individual element given the value of its id attribute.
- `querySelector` uses CSS selector syntax that would select one or more elements.
### Methods That Return One or More Elements
- `getElementsByClassName` selects one or more elements given the value of their class attribute.
- `getElementsByTagName` selects all elements on the page with the specified tag name.
- `querySelectorAll` uses CSS selector syntax to select one or more elements and returns all of those that match.

- the `item()` method will return an individual node from the Node list.
- **array syntax** is preferred over the item() method because it is faster. You can access individual nodes using a square bracket syntax similar to that used to access individual items from an array.
```javascript
var hotItems = document.querySelectorAll('li.hot');
for (var i = 0; i < hotItems.length; i++) {
  hotItems[i].className = 'cool';
}
```
- the variable `hotItems` contains a nodelist. It contains all list items whose class attribute has a value of hot.
- the length property of the node list indicates how many elements are in the node list.
- array syntax is used to indicate which item in the nodelist is currently being worked with: `hotItems[i]`
- when you have an element node, you can select another element in relation to it using these five properties:
1. `parentNode` finds the element node for the containing element in the HTML.
2. `previousSibling` or `nextSibling` find the previous or next sibling of a node.
3. `firstChild` or `lastChild` find the first or last child of the current element.

#### Adding or Removing HTML Content

- there are two different approaches to adding and removing content from a dom tree: the innerHTML property and dom manipulation.
- **innerHTML** can be used on any element node. It is used both to retrieve and replace content. Example:
```javascript
var item;
item = '<em>Fresh</em> figs';
```
1. create variable holding markup
2. select element whose content you want to update.
3. Update content of selected element with new markup
- **dom manipulation** easily targets individual nodes in the dom tree whereas innerHTML is better suited to updating entire fragments. Example:
1. Create a new text node `text`
2. Create new element node `li`
3. add text node to element node `li`---> `text`.
4. select element you want to add the new fragment to
5. append the new fragment to the selected element.

- once you have an element node, you can use other properties and methods on that element node to access and change its attributes.
1. select the element node that carries the attribute and follow it with a period symbol.
2. Then use one of the methods or properties below to work with that elements attributes.
`document.getElementById('one').getAttribute('class');`

[<===Home](README.md)