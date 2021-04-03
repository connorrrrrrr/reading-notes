## Thinking in React

- you'll want to draw boxes around every componet and subcomponet in the mock and give them all names.

- if you're not sure what should be its own componet, use the **single responsibility principle** (a componet should ideally only do one thing, if it ends up growing, it shoudl be decomposed into smaller subcomponets).

- when you have your componet hierarchy, you can implement your app. The easiest way is to build a version that takes your data model and renders the UI but has no interactivity.

- to build a static version of your app that renders your data model, you'll need to build componets that reuse other componets and pass data using **props**.

- to make UI interactive, you need to be able to trigger changes to your underlying data model. React does this with **state**.

- to build your app correctly, you need to first think of the minimal set of mutable state that your app needs.

- go through each piece of data and ask three questions:

1. Is it passed in from a parent with props? If so, it probably isn't state.

2. Does it remain unchanged over time? If so, it probably isn't state.

3. Can you compute it based on any other state or props in your componet? If so, it isn't state.

For each piece of state in your application:

- identify every componet that renders something based on that state.

- find a common owner componet (a single componet above all).

- either the common owner or another componet higher up in the hierarchy should own the state.

- if you can't find a componet where it makes sense to own the state, create a new componet solely for holding the state and add it somewhere in the hierarchy above the common owner componet.

[<===Home](README.md)