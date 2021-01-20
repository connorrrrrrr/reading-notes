# CSS Layout
- CSS treats each HTML element as if it's in its own box.
- **block level** elements start on a new line.
  - ex: `<h1>` or `<p>`
- **inline elements** flow in between surrounding text.
  - ex: `<img>`
- if one block level element sits inside another block level element then the outer box is known as the **containing** or **parent** element.
- CSS has the following **positioning schemes** that allow you to control the layout of a page:
  1. Normal Flow
    - every **block level** element appears on a new line, causing each item to appear lower down the page than the previous one.
  2. Relative Positioning
    - this moves an element from the position it would be in a normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.
  3. Absolute Positioning
    - this positions the element in relation to its containing element. It's taken out of normal flow, meaning that it doesn't affect the position of any surrounding elements.
    - these elements move as users scroll up and down the page.
  4. Fixed Positioning
    - this is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element.
  5. Floating Elements
    - floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box.
- different visitors to your site will have different screen sizes.
- because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide.
- **fixed width layout** designs do not change size as the user increases or decreases the size of their browser window.
- **liquid layout** designs stretch and contract as the user increases or decreases the size of their browser.
- the `float` property moves content to the left or right of the page and can be used to create multi column layouts.

[<===Home](README.md)