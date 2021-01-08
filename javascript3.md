## Comparison Operators

1. == - is equal to
    - this operator compares two values to see if they are the same
2. != - is not equal to
    - this operator compares two values to see if they are _not_ the same
3. === - strict equal to
    - this operator compares two values to check that both the data type and value are the same
4. !== - strict not equal to
    - this operator compares two values to check that both the data type and value are _not_ the same

## Logical Operators

```javascript
((5 < 2) && (2 >= 3))
```
In this one line of code there are 3 expressions, each of which will resolve to the value true or false. The expressions on the left and right both use comparison operators, and both return false. The third expression uses a logical operator. The logical && operator checks to see whether both expressions on either side of it return true.

1. && - logical and
    - this operator tests more than one condition.
2. || - logical or
    - this operator tests at least one condition.
3. ! - logical not
    - this operator takes a single boolean value and inverts it.

## Loops

Loops check a condition. If it returns ture, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. It repeats until the condidion returns false. Three common types of loops are:

1. For loop
    - this is used for running code a specific number of times.
2. While loop
    - if you don't know how many times the code should run, this is what you should use. This allows the condition to be something other than a counter, and the code will continue to loop for as long as the condition is true.
3. Do While loop
    - this is very similar to the while loop, but has one key difference: it will always run the statements inside the curly braces at least once, even if the condition evaluates to false.


[<===Home](README.md)