## Text

- **Structural markup**: the elements that you can use to describe both headings and paragraphs.
- **Semantic markup**: provides extra information such as: where emphasis is placed in a sentence, that someting you have written is a quotation, the meaning of acronyms, etc.

1. H1, H2, H3, H4, H5, H6
  - six levels of headings
2. p
  - used for paragraphs
3. b
  - makes text bold
4. i
  - makes text italic
5. sup
  - used to contain characters that should be superscript such as the suffixes of dates or mathematilcal concepts like raising a number to a power.
6. sub
  - used to contain characters that should be subscript.
7. br /
  - break line tag, used for adding line breaks inside the middle of paragraphs.
8. hr /
  - used to add a horizontal line to seperate sections
9. strong
  - used similar to bold. Indicates that its content has strong importance.
10. em
  - indicates emphasis that subtly changes the meaning of a sentence. Used similarly to italic.
11. blockquote
  - used for longer quotes that take up an entire paragraph.
12. q
  - used for shorter quotes that sit within a paragraph.
13. abbr
  - used for abbreviations or acronyms.
14. cite
  - used for referencing a piece of work.
15. dfn
  - used for indicating the defining instance (the first time you explain some new terminology).
16. address
  - used to contain contact details for the author of the page.
17. ins and del
  - the **ins** can be used to show content that has been inserted into a document. The **del** can show text that has been deleted from it. Ins underlines and del crosses out.
18. s
  - indicates something is no longer accurate or relevant (but that should't be deleted).

## CSS

The key to understanding how CSS works is to imagine every HTML element is surrounded by a box. CSS allows you to create rules that control the way that each individual box is presented. CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

**Selectors** indicate which element the rule applies to.

**Declarations** indicate how the elements referred to in the selector should be styled.

```css
p {
  font-family: Arial;}
```
CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon. **Declarations** are made up of two parts: the properties of the element that you want to change, and the values of those properties.

**Properties** indicate the aspects of the element you want to change.

**Values** specify the settings you want to use for the chosen properties.

1. '<link>'
  - can be used in an HTML document to tell the browser where to find the CSS file used to style the page. Used with 'href', 'type', and 'rel'.
2. '<style>'
  - used for including CSS rules within an HTML page. Usually sits in the '<head>' element.

## Javascript

Each individual instruction of a script is called a **statement**. Statements should end with a semicolon. Some statements are surrounded by curly braces, these are known as **code blocks**. 

#### Variables

1. Before you can use a variable, you need to announce that you want to use it. You also must give it a name.
2. Once you have created a variable, you can tell it what information you would like it to store for you. Use an equals sign to assign it a value.
```javascript
var quantity = 3;
```
**Rules for naming variables**.
1. The name must begin with a letter, dollar sign ($),or an underscore (_). 
2. The name can contain letters,numbers, dollar sign ($), or an
underscore (_).
3. You cannot use keywords or reserved words.
4. All variables are case sensitive.
5. Use a name that describes the kind of information that the variable stores.
6. If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word.

An **array** is a special type of variable. It doesn't just store one value; it stores a list of values. Consider using this when you are working with a list or a set of values that are related to each other. You create an array and give it a name just like you would any other variable.
```javascript
var colors;
colors = ['white', 'black', 'custom'];
```
You can also create arrays using a technique called an array constructor.
```javascript
var colors = new Array('white',
                        'black', 
                        'custom');
```

Javascript distinguishes between numbers (0-9), strings (text), and Boolean values (true or false). Expressions evaluate into a single value and they rely on operators to calculate a value. 

### Decisions and Loops

There are two componets to a decision:
1. An expression is evaluated and returns a value
2. A conditional statement says what to do in a given situation.

Evaluation of a condition is commonly done by comparing two values using a **comparison** operator. There are multiple comparison operators.
1. '=='
  - is equal to
2. '!='
  - is not equal to
3. '==='
  - strict equal to. This operator compares two values to check that both the data type and value are the same.
4. '!=='
  - strict not equal to. This operator compares two values to check that both the data type and value are _not_ the same.
5. '>'
  - greater than
6. '<'
  - less than
7. '>='
  - greater than or equal to
8. '<='
  - less than or equal to

In any condition, there is usually one operator and two operands. The operands are placed on each side of the operator. They can be values or variables.
```javascript
(score >= pass)
```
In this example, the operands are 'score' and 'pass'. The comparison operator is greater than or equal to. The operand doesn't have to be a single value or variable name. It can be an _expression_ as well.
```javascript
((score1 + score2) > (highScore1 + highScore2))
```
**Logical Operators**

While comparison operators usually return single values of true or false, logical operators allow you to compare the result of more than one comparison operator. 

1. '&&'
  - logical and. This operator tests more than one condition.
2. '||'
  - logical or. This operator tests at least one condition.
3. '!'
  - logical not. This operator takes a single boolean value and inverts it.

The **if** statement evaluates a condition. If the condition evaluates to true, any statements in the subsequent code block are executed.
  ```javascript
  if (score >= 50) {
    congratulate();
  }
  ```
The **if else** statement checks a condition. If it resolves to true the first code block is executed. If the condition resolves to false the second code block is ran instead.
```javascript
if (score >= 50) {
  congratulate();
}
else {
  encourage();
}
```
In this example, the code to execute if value is true would be congratulate. If the value is false, encourage.

[<===Home](README.md)