# Intro to CSS

Imagine there is a block around every HTML element. CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

**Examples**

* Boxes
* Text
* Specifics

## Common Elements

* the **link** element can be used in an HTML document to tell the browser where to find the CSS file used to style the page, does not need a closing tag. Lives inside (head) element.
* **href** specifies the path to the CSS file. Often placed in a folder called "css" or "styles".
* the **type** attribute specifies the type of document being linked to.
* **rel** specifies the relationship between the HTML page and the file it is linked to. The value should be "stylesheet" when linking to a CSS file.
* you can include CSS rules within an HTML page by placing them inside a **style** element. Usually sits inside the *head* element of the page.

```text
<style type="text/css">
```

## Using Color

You can specify any color in CSS in one of the three ways:

- RGB Values
    - these express colors in terms of how much red, green, and blue are used to make it up. Example: rgb(100.100.90)
- Hex Codes
    - six digit codes that represent the amount of red, green, and blue in a color, preceded by a pound. Example: #ee3e80
- Color Names
    - there are 147 predefined color names that are recognized by browsers.
- HSL
    - has been introduced in CSS3 as an alternative way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for: HUE(between 0 and 360 degrees), Saturation(exposed as percentage), and Lightness(expressed as a percentage with 0% being white and 100% being black).

**Color Pickers can tremendously help you find the color you want.**

You can specify background color by using:
```text
body {
background-color: rgb(200,200,200);}
```

When picking font and background color, it is most important to ensure that the text is easily legible. CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements.

Example:
```text
body {
background-color: rgb(0.0.0);
opacity: 0.5;}
```
