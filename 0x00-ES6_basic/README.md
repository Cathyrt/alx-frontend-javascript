# 0x00-ES6_basic

ES6, also known as ECMAScript 2015, is the sixth major version of the ECMAScript language specification. It introduced several new features and improvements to JavaScript, enhancing its capabilities and making code more concise and expressive.

## New Features introduced in ES6

ES6 introduced many new features. Some of the prominent ones are:

- **Arrow Functions:** Arrow functions provide a more concise syntax for writing functions and automatically bind the `this` value based on the surrounding context.

- **Block-scoped Variables:** `let` and `const` were introduced to declare block-scoped variables, allowing better control over variable scoping.

- **Default Function Parameters:** ES6 allows defining default values for function parameters, simplifying function declarations and reducing the need for manual argument checks.

- **Rest and Spread Parameters:** The rest parameter (`...`) allows a function to accept any number of arguments as an array, while the spread operator (`...`) spreads an array into individual arguments.

- **Template Literals:** ES6 introduced template literals, allowing the embedding of expressions inside string literals using `${}` syntax. This enables easy string interpolation and multiline strings.

- **Enhanced Object Literals:** ES6 introduced new syntax for object creation and manipulation, including shorthand property names, computed property names, and concise method syntax.

- **Iterators and for-of Loops:** Iterators provide a standard way to iterate over collections. The `for-of` loop was introduced as a concise syntax for iterating over iterable objects.

## Constants vs Variables

In JavaScript, a variable is a named storage location that can hold different values throughout its lifetime. On the other hand, a constant is a variable-like entity that can only be assigned once and cannot be reassigned.

The main differences between constants and variables are:

- **Assignment:** Variables can be assigned multiple times, while constants can only be assigned once during their declaration.

- **Mutability:** Variables can be mutated, meaning their value can change over time. Constants, however, are immutable and cannot be reassigned after the initial assignment.

- **Scope:** Both variables and constants have scope, but constants have block scope when declared using `const` within a block, while variables declared with `var` have function scope.

## Block-scoped Variables

Block-scoped variables were introduced in ES6 with the `let` and `const` keywords. Unlike variables declared with `var`, block-scoped variables are limited to the nearest enclosing block or statement. They are not hoisted to the top of their scope and are accessible only within their respective block.

The block-scoped variables have the following characteristics:

- They are not accessible outside their block.

- They are not hoisted to the top of their scope.

- They follow the temporal dead zone (TDZ) rules, meaning they can't be accessed before their declaration.

## Arrow Functions and Default Function Parameters

Arrow functions in ES6 provide a concise syntax for writing functions. They have the following features:

- They have a shorter syntax compared to traditional function expressions.

- They inherit the `this` value from the surrounding context, eliminating the need to bind `this` explicitly.

- They cannot be used as constructors or have their own `arguments` object.

ES6 also introduced default function parameters, allowing developers to specify default values for function arguments. If a parameter is not passed when invoking the function, the default value will be used instead.

## Rest and Spread Function Parameters

Rest parameters and spread syntax were introduced in ES6. They have similar syntax but are used in different contexts:

- **Rest Parameters:** The rest parameter (`...`) allows a function to accept any number of arguments as an array. It is used in function definitions to gather a variable number of arguments into an array.

- **Spread Syntax:** The spread syntax (`...`) spreads an array into individual elements. It is used in function calls or array literals to expand an array into multiple arguments or elements.

## String Templating in ES6

ES6 introduced template literals, also known as string interpolation or string templating. They provide an elegant way to embed expressions within string literals. Template literals are enclosed by backticks (``) instead of single or double quotes. Expressions within template literals are enclosed in `${}`.

Template literals offer the following advantages:

- String interpolation: Expressions can be directly embedded within the string, eliminating the need for concatenation.

- Multiline strings: Template literals can span multiple lines without requiring escape characters or string concatenation.

## Object Creation and Properties in ES6

ES6 introduced several enhancements to object creation and manipulation. Some key features include:

- **Shorthand Property Names:** Objects can be defined with shorthand property names, allowing you to define properties without explicitly specifying their values.

- **Computed Property Names:** ES6 introduced the ability to use expressions for property names by wrapping them in square brackets (`[]`).

- **Concise Method Syntax:** Object methods can be defined using concise syntax, omitting the `function` keyword.

## Iterators and for-of Loops

ES6 introduced the concept of iterators, which provide a standardized way to iterate over collections. Iterators allow objects to define their iteration behavior, enabling the use of the `for-of` loop to iterate over iterable objects.

The `for-of` loop is a convenient and concise syntax for iterating over elements of an iterable object, such as arrays, strings, or custom objects that implement the iterable protocol.

---
