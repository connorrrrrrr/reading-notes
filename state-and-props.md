## State and Props
- react events are named using camel case.
- with JSX you pass a function as the event handler rather than as a string.
- you can't return false to prevent default behavior in react. You must call preventDefault explicitly.
- **conditional rendering** in React works the same way conditions work in JavaScript.
- you can use variables to store elements.
- you can embed expressions in JSX by wrapping them in curly braces. Includes the logical && operator.
- In some cases you might want a componet to hide itself even though it was rendered by another componet. You can do this by returning `null` instead of its render output.
- returning `null` from a componet's `render` method does not affect the firing of the componet's lifecycle methods.
- the `render` method returns a description of what you want to see on the screen, react takes the description and displays the result.

[<===Home](README.md)