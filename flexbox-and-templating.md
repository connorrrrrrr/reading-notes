## JavaScript Templating

- javascript templating is a technique used to render client-side view templates with javascript by using  a json data source.
- the template is html markup.
### Mustache
- Mustache is a logic-less template syntax.
- used for html, config files, source code- anything.
- no if statements, else clauses, or for loops.
```Javascript
Mustache.render("hello, {{name}}", { name: "Sherlynn" });
```
- in the above, there are two braces around name. This is mustache syntax to show that it is a placeholder. When Mustache compiles it, it will look for the 'name' property in the object we pass in, replacing {{name}} with the actual value, "Sherlynn".
## Flexbox
- the main idea behind the flex layout is to give the container the ability to alter its items width/height to best fill the available space.
- flexbox involves a lot of things including its whole set of properties.
- some of them are meant to be set on the container whereas the others are meant to be set on the children.
- **main axis** - the main axis of a flex container is the primary axis along whcih flex items are laid out.
- **main-start**|**main-end** - flex items are placed within the container starting from main-start to main-end.
- **main size** - on a flex item's width or height, whichever is the main dimension is the item's main size. Will be either width or height dimension for the main dimension.
- **cross axis** - the axis perpendicular to the main axis.
- **cross-start**|**cross-end** - flex lines are filled with items and placed into the container starting on the cross-start side of the flex container and going toward the cross-end side.
- **cross size** - the width or height of a flex item, whichever is in the cross dimension is the item's cross size.

[<===Home](README.md)