### Lifting State Up

- at times, several componets need to reflect the same changing data. It is recommended to lift the shared state up to their closest common ancestor.

- usually, the state is added first to the componet that needs it for rendering. Then if other componets need it, you can lift it lup to their closest common ancestor. Rely on the top-down data flow.

- since any state "lives" in a componet and that componet alone can change it, the surface area for bugs is significantly reduced. You can implement any custom logic to reject or transform user input. If something can be derived from either props or state, it probably shouldn't be in the state.

#### Keys

- a **key** is a string attribute you need to include when creating lists of elements.

- keys help React identify which items have changed, are added, or are removed.

- keys that are used within arrays should be unique among their siblings, but they don't need to be globally unique. The same keys can be used when producing two different arrays.

### Spread Operator

- In JavaScript, the **spread** syntax refers to the use of an ellipsis of three dots (...) to expand an iterable object into the list of arguments.

The `...` spread operator is useful for the following tasks in JS:

- copying an array
- concatenating or combining arrays
- using math functions
- using an array as arguments
- adding an item to a list
- adding to state in React
- combining objects
- converting NodeList to an array

[<===Home](README.md)