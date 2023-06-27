# 0x01. ES6 Promises

This guide provides an overview of Promises, the `await` operator, and async functions in JavaScript.

## Promises

### What are Promises?
Promises are a way to handle asynchronous operations in JavaScript. They represent the eventual completion or failure of an asynchronous task and allow you to attach callbacks to handle the results.

### Why use Promises?
Promises help avoid callback hell and make asynchronous code more readable and maintainable. They provide a way to handle success and error cases separately and enable chaining of asynchronous operations.

### How to use Promises?
To create a Promise, you can use the `Promise` constructor, which takes a function (often called the executor) with two parameters: `resolve` and `reject`. Inside the executor, you perform your asynchronous task and call `resolve` when it succeeds or `reject` when it fails.

The `then` method is used to attach a callback that executes when the Promise is resolved. It takes two optional parameters: `onFulfilled` and `onRejected`. You can chain multiple `then` calls together to handle the asynchronous operations sequentially.

The `catch` method is used to attach a callback that executes when the Promise is rejected. It is typically used to handle errors thrown during the Promise's execution.

## Promise Methods

### Using the `then`, `resolve`, and `catch` methods
The `then` method is used to handle the resolved value of a Promise. It takes a callback function as its parameter, which receives the resolved value. The `resolve` method is used inside the Promise executor to fulfill the Promise with a value.

The `catch` method is used to handle errors or rejections that occur during the Promise's execution. It takes a callback function as its parameter, which receives the error object.

### Using the `every` method of the Promise object
The `every` method is not a built-in method of the Promise object in JavaScript. It seems you might be referring to a different concept or library. Please provide more context or clarify the specific functionality you are referring to.

## Error Handling

### Throw / Try
The `throw` statement is used to manually throw an exception. It is typically used within a `try...catch` block. The `try` block contains the code that might throw an exception, and the `catch` block handles the thrown exception by specifying the type of error to catch and the code to execute when the error occurs.

## Async/Await

### The `await` operator
The `await` operator is used to wait for a Promise to resolve or reject before continuing with the execution of the surrounding `async` function. It can only be used inside an `async` function. When `await` is used, it pauses the execution of the function until the Promise settles, and then it returns the resolved value or throws the rejected value as an exception.

### Using an async function
An `async` function is a function that implicitly returns a Promise. It allows you to write asynchronous code in a more synchronous-like manner. Inside an `async` function, you can use the `await` operator to wait for Promises to settle, making it easier to handle asynchronous operations.

To use an async function, you define it using the `async` keyword before the function declaration. The function body can contain `await` expressions to pause execution and wait for Promises to resolve.

## Conclusion
Promises, along with the `then`, `resolve`, `catch` methods, error handling with `throw` and `try...catch`, and the async/await syntax provide powerful tools for working with asynchronous JavaScript code. They improve code readability, maintainability, and help avoid common pitfalls associated with callback-based asynchronous programming.

