## Forms

- HTML form elements work differently from other DOM elements in React because form elements naturally keep some internal state. Elements such as `<input>`, `<textarea>`, and `<select>` usually maintain their own state and update it based on user input. In react, mutable state is usually kept in the state property of componets and only updated with `setState()`.

- with a controlled componet, the input's value is always driven by the React state.

- in HTML, an `<input type="file">` lets the user choose one or more files from their device storage to be uploaded to a server or manipulated by JavaScript with the File API. Its value is read-only so it is an **uncontrolled** componet in React.

- when you need to handle multiple controlled `input` elements, you add a `name` attribute to each element and let the handler function choose what to do based on the value of `event.target.name`.

[<===Home](README.md)