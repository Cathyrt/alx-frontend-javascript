# ES6 Data Manipulation

This repository provides a brief introduction to ES6 data manipulation techniques, including the usage of map, filter, and reduce on arrays, as well as an overview of typed arrays and the Set, Map, and WeakLink data structures.

## Table of Contents

- Array Manipulation
  - Map
  - Filter
  - Reduce
- Typed Arrays
- Data Structures
  - Set
  - Map
  - WeakLink

## Array Manipulation

### Map

The `map` method is used to transform each element of an array into a new element based on a provided callback function. It returns a new array with the transformed elements. Here's an example:

```
const numbers = [1, 2, 3, 4, 5];
const doubledNumbers = numbers.map((num) => num * 2);

console.log(doubledNumbers); // Output: [2, 4, 6, 8, 10]
```

### Filter

The `filter` method is used to create a new array containing only the elements that satisfy a certain condition specified by a callback function. It returns a new array with the filtered elements. Here's an example:

```
const numbers = [1, 2, 3, 4, 5];
const evenNumbers = numbers.filter((num) => num % 2 === 0);

console.log(evenNumbers); // Output: [2, 4]
```

### Reduce

The `reduce` method is used to iterate over an array and accumulate the values into a single result. It takes a callback function and an optional initial value. The callback function receives an accumulator and the current element, and returns the updated accumulator value. Here's an example:

```
const numbers = [1, 2, 3, 4, 5];
const sum = numbers.reduce((accumulator, num) => accumulator + num, 0);

console.log(sum); // Output: 15
const numbers = [1, 2, 3, 4, 5];
const sum = numbers.reduce((accumulator, num) => accumulator + num, 0);

console.log(sum); // Output: 15
```

## Typed Arrays

Typed arrays provide a way to work with binary data in JavaScript. They allow you to store and manipulate data in a specified format, such as 8-bit integers, 16-bit integers, and floating-point numbers. Typed arrays have better performance characteristics compared to regular arrays when dealing with binary data. Here's an example of creating and working with a typed array:

```
const buffer = new ArrayBuffer(16);
const int32Array = new Int32Array(buffer);
int32Array[0] = 42;
int32Array[1] = 23;

console.log(int32Array); // Output: Int32Array [42, 23]
```

## Data Structures

### Set

The `Set` data structure is an unordered collection of unique values. It allows you to store any type of value and provides methods to add, remove, and check for the presence of elements. Here's an example:

```
const set = new Set();
set.add(1);
set.add(2);
set.add(3);

console.log(set.size); // Output: 3
console.log(set.has(2)); // Output: true
set.delete(2);
console.log(set.size); // Output: 2
```

### Map

The `Map` data structure is a collection of key-value pairs, where each key is unique. It provides methods to add, retrieve, and remove elements based on their keys. Here's an example:

```
const map = new Map();
map.set('name', 'John');
map.set('age', 30);

console.log
```

### WeakLink

The `WeakLink` data structure is similar to `Map`, but it allows keys to be garbage collected if there are no other references to them. This can be useful in scenarios where you want to associate additional data with an object without preventing its memory from being freed. Here's an example:

```
const weakMap = new WeakMap();
let key = {};

weakMap.set(key, 'value');
console.log(weakMap.get(key)); // Output: value

key = null; // Clearing the reference
// The entry in weakMap can now be garbage collected

console.log(weakMap.get(key)); // Output: undefined
```

---
