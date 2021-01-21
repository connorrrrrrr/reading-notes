## Forms
1. A user fills in a form and then presses a button to submit the information to the server.
2. The name of each form control is sent to the server along with the value the user enters or selects.
3. The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information.
4. The server creates a new page to send back to the browser based on the information received.
- a form may have several form controls, each gathering different information.
- `<form>` is where form controls live. This element should always carry the `action` attribute.
  - forms can be sent using one of two methods: **get** or **post**.
  - with the **get** method, the values from the form are added to the end of the URL specified in the action attribue. Use this for: short forms such as search boxes or when you are just retrieving data from the web server.
  - with the **post** method, the values are sent in what are known as HTTP headers. Use this if your form: allows users to upload a file, is very long, contains sensitive data, adds information to, or deletes information from a database.
- `<input>` is used to create several different form controls.
  - the value of the `type` attribute determines waht kind of input they will be creating.
  - you can use `maxlength` to limit the number of characters a user may enter into the text field.
  - the `name` attribute indicates the name of the password input, which is sent to the server with the password the user enters.
  ```html
<form action="http://www.example.com/login.php">
  <p>Username:
    <input type="text" name="username" size="15"
    maxlength="30">
  </p>
  <p>Password: 
    <input type="password" name="password" size="15"
  maxlength="30" />
  </p>
</form>
```

- `<textarea>` is used to create a multi-line text input.
- `type="radio"` allows users to pick just one from a number of options.
- `type="checkbox"` allows users to select and unselect one or more options in answer to a question.
- `<select>` is a drop down list, contains two or more options.
  - `<option>` is used inside the select element to specify the options that the user can select from.
- `type="file"` creates a box that looks like a text input followed by a browse button. Allows users to upload files to the site.
- `type="submit"` is used to send a form to the server.
- `type="image"` is used to use an image for the submit button.
- `<label>` is used to label the options the user has.
- `<fieldset>` is used to group related form controls together.
  - `<legend>` can come directly after the opening fieldset tag and contains a caption.
- `type="date"` is used for asking the user to enter a date.
- `type="email"` is used for asking user for their email.
- `type="search"` is used to create a text box for search queries.

#### Lists and Tables
- `list-style-type` allows you to control the shape or style of a bullet point.
- `list-style-image` allows you to specify an image to act as a bullet point.
- shading every other row of your table can help users read it.
- if you have empty cells in your table, then you can use `empty-cells` to specify whether or not their border should be shown.

## Events

- events are the browser's way of indicating when something has happened.
- **binding** is the process of stating which event you are waiting to happen, and which element you are waiting for that to happen upon.
- some different event types are: **ui events**(ex: when a user has scrolled up or down the page), **keyboard events**(ex: pressing a key), and **mouse events**(ex: interacting in the web page with your mouse).
- when a user interacts with the HTML, there are three steps involved in getting it to trigger some Javascript code.
1. select the element noede(s) you want the script to respond to
2. indicate which event on the selected node(s) will trigger the response
3. state the code you want to run when the event occurs.
- html elements nest inside other elements. If you hover or click on a link, you will also be hovering or clicking on its parent elements.
- the **event** object can tell you where the cursor was positioned when an event was triggered.

[<===Home](README.md)