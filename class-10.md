# Error Handling & Debugging

- Execution context - every statement in a script lives in one of the three execution contexts:
  - global context
  - function context
  - eval context 
- variable scope
  - global scope
  - function-level scope
- The Javascript interpreter processes one line of code at a time. When a statement needs data from another function, it stacks the new function on top of the current task. 
- in the interpreter, each execution context has its own variables object.
- if a javascript statement generates an error, then it throws an **exception**. At that point, the interpreter stops and looks for exception handling code.
- debugging is the process of finding errors, involves the process of deduction.
- Javascript has 7 different type of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.
### Error Objects

- error
  - generic error- the other errors are based upon this one
- syntax error
  - syntax has not been followed
- reference error
  - tried to reference a variable that is not declared/within scope.
- type error
  - an unexpected data type that cannot be coerced.
- range error
  - numbers not in acceptable range
- uri error
  - encodeURI(), decodeURI(), and similar methods used incorrectly
- eval error
  - eval() function used incorrectly

[<===Home](README.md)