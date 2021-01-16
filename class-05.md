## Images

- `<img>`
  - to add an image into the page you need to use this.
    - `src`: tells the browser where it can find the image file.
    - `alt`: provides a text description of the image.
    - `title`: attribute that provides additional information about the image.
    - `height`: specifies height in pixels
    - `width`: specifies width in pixels
- `<figure>`: this is used to contain images and thier captions so they are associated.
- `<figcaption>`: this is where you put your caption at.
- Photographs are best saved as **JPEG**; logos that use flat color should be saved as **GIF**.

## Color

- `color`: this property allows you to specify the color of text inside an element.
  - you can specify colors by using, rgb values, hex codes, or predefined color names.
- `background-color`: this is what you use to color the background of an element.
- every color on a computer screen is created by mixing amounts of red, green, and blue.
- **saturation** is the amount of gray in a color.
- **brightness** refers to how much black is in a color.
- `opacity`: allows you to specify the opacity of an element and any of its child elements.
- `hsl` or `hsla`: are color properties that start with `hsl` followed by:
  - **HUE** (expressed as an angle between 0 and 360 degrees)
  - **Saturation** (expressed as a percentage)
  - **Lightness** (expressed as a percentage)
  - **Alpha** is used if you're using `hsla`, this is expressed as a number between 0 and 1. For example: 0.5 represents 50% transparency.
- it is important to ensure that there is enough contrast between any text and the background color.

## Text

- **serif** fonts have extra details on the ends of the main strokes of the letters. (times new roman)
- **sans-serif** fonts have straight ends to letters. (arial)
- **monospaced** have the exact same width for each character.
- there is a limited choice of fonts that you can assume most people will have installed.

- the **weight** of the font specifies the boldness of characters
  - `font-weight`
- the **style** of the font specifies the cursive aspect to some of the lettering (italic)
  - `font-style`: can be used to make text italic or oblique.
- the **stretch** of the font specifies the thickness and how close or far apart the characters are.

- `font-family`: this property allows you to specify the typeface (font) that should be used for any text within the element.
- `font-size`: this property enables you to specify a size for the font using **pixels**, **percentages**, or **em**.
  - an **em** is equivalent to the width of the letter 'm'.
  - pixels are the most precise way to size text
- the default size of text in a browser is 16 pixels.
- `@font-face`: this allows you to use a font even if it's not installed on the computer of the person browsing.
  - with `font-family`, you can use this name as a value after you put it in the `@font-face` property. Example:

```css
@font-face {
  font-family: 'ChunkFiveRegular';
  src: url('urlgoeshere.com');
}
h1, h2 {
  font-family: ChunkFiveRegular, Georgia, serif;}
```
- `text-transform`: this property is used to change the capitalization of text.
  - **uppercase** causes all text to appear uppercase
  - **lowercase** causes all text to appear undercase
  - **capitalize** causes the first letter of every word to be capitalized.
- `text-decoration` allows you to specify:
  - **none** removes any decoration already appplied to text.
  - **underline** adds a line underneath.
  - **overline** adds a line over the top.
  - **line-through** adds a line through.
  - **blink** animates the text to flash on and off (this is generally frowned upon)
- `line-height` sets the height of an entire line of text. Increasing this makes the vertical gap between lines of text larger.
- `text-align`: this allows you to control the alignment of text using: left, right, center, and **justify**.
  - **justify** indicates that every line in a paragraph, except for the last line, should be set to take up the full width of the containing box.
- `text-indent`: this property allows you to indent the first line of text within an element. It can take negative values, which means it can be used to push text off the browser window.
- `:first-letter`, `:first-line`: these are known as **pseudo-elements**. You can specify different values for the first letter or first line of text inside an element.

[<===Home](README.md)