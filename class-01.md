# HTML

HTML pages are text documents. HTML code is made up of characters that live inside angled brackets (<>). These are called HTML **elements**. Elements are usually made up of two **tags**: an opening and closing tag (<>). The closing tag has an extra forward slash (/) in it. Each HTML element tells the browser something about the information that is in between its opening and closing tags (<>). HTML uses elements to describe the structure of web pages. Tags are like containers that tell you something about the information that lies between each <>. To learn HTML you need to know what tags are available for you to use, what they do, and where they can go.

**Attributes** give you more information about the contents of an **element**. An attribute is made of two parts: a _name_ and a _value_ sperated by an equal (=) sign.
```html
<p lang="en-us"> Paragraph in English</p>
```
The attribute _name_ indicates what kind of extra information you are supplying about the element's content. The _value_ is the information or setting for the attribute. It should be placed in double quotes. Here an attribute called _lang_ is used to indicate the language used in this element. The value ("en-us") specifies that it is in US English.

### Escape Characters

There are some characters that are used in and reserved by HTML code.

1. Less than sign
    - &lt;
    - &#60;
2. Greater than sign
    - &gt;
    - &amp;
3. Ampersand
    - &amp;
    - &#38;
4. Quotation mark
    - &quot;
    - &#34;
5. Cent sign
    - &cent;
    - &#162;
6. Pound sign (not #)
    - &pound;
    - &#163;
7. Yen sign
    - &yen;
    - &#165;
8. Euro sign
    - &euro;
    - &#8364;
9. Copyright symbol
    - &copy;
    - &#169;
10. Registered trademark
    - &reg;
    - &#174;
11. Trademark
    - &trade;
    - &#8482;
12. Left single quote
    - &lsquo;
    - &#8216;
13. Right single quote
    - &rsquo;
    - &#8217;
14. Left double quotes
    - &ldquo;
    - &#8220;
15. Right double quotes
    - &rdquo;
    - &#8221;
16. Multiplication sign
    - &times;
    - &#215;
17. Division Sign
    - &divide;
    - &#247;

**Doctypes** tell browsers which version of HTML you are using. You can add comments to your code between <!-- and --> markers. The _id_ and _class_ attributes allow you to identify particular elements. The **div** and **span** elements allow you to group block level and inline elements together. Iframes cut windows into your web pages where other web pages can be displayed. The **meta** tag allows you to supply information about your webpage.

HTML5 added more elements to provide clearer code. They indicate the purpose of different parts of a web page and help to describe its structure. Some of the elements include:

1. Header and footer
    - the main header or footer that appears at the top or bottom of every web page.
2. Navigation
    - the nav element is used to contain the major navigational blocks on the site.
3. Articles
    - the article element acts as a container for any section of a page that could stand alone.
4. Asides
    - the aside element has two purposes depending if its inside an article element or not. When inside an article, it should contain information that is related to the article. When outside, it acts as a container for content that is related to the entire page.
5. Section
    - the section element groups related content together.
6. Heading Groups
    - grouping elements with h1,h2,h3, etc.
7. Figures
    - used for images, videos, graphs, diagrams, code samples, text that supports the main body of an article.

It's important to understand who your audience is, why they would come to your site, what information they want to find, and when are they likely to return. Using **site maps** and **wireframes** you can plan the structure and organize the information that needs to go on each page. Visual hierarchy helps visitors understand what you're trying to tell them. It helps to differentiate information by size, color, and style. It is also important to simplify the information you present.

# Javascript

A **script** is a series of instructions that a computer can follow to achieve a goal. To write one, you need to first state your goal and then list the tasks that need to be completed in order to achieve it. Start with a big picture, then break it down into multiple steps. "Thinking" like a computer is important. Try sketching out the tasks in a flow chart. Objects can have: properties that tell us about the object; methods that perform tasks using properties of the object; events which are triggered when a user interacts with the computer.

### How a Browser Sees a Web Page

1. Recieve page as HTML code
2. Create a model of the page and store it in memory.
3. Use a rendering engine to show the page on screen.

All major browsers use a javascript interpreter to translate your instructions (in javascript) into instructions the computer can follow. 
```Javascript
document.write('Good Afternoon!');
```
The _document_ **object** represents the entire web page. The _write()_ **method** of the _document_ object allows new content to be written into the page where the **script** element sits. Javascript runs where it is found in the HTML. This is where you use the **script** element. It is best to keep javascript code in its own javascript file. Using the .js extension.

[<===Home](README.md)