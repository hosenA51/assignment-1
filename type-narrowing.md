# Type Narrowing in TypeScript: typeof, instanceof, and the in Operator

## Introduction

A union type allows a variable to hold values of more than one type. Before using a value, TypeScript needs enough information to know which operations are safe. Type narrowing is the process of reducing a broad type to a more specific type through checks in the code.

## Detailed Explanation

The `typeof` operator is useful for JavaScript primitive types such as strings, numbers, and booleans. TypeScript understands the condition and narrows the variable inside each branch.

The `instanceof` operator checks whether an object was created from a particular class or constructor. It is useful when a function accepts instances of different classes.

The `in` operator checks whether a property exists on an object. TypeScript can use that check to distinguish object types in a union.

## Conclusion

Type narrowing makes union types practical and safe. Use `typeof` for primitive values, `instanceof` for class instances, and `in` to distinguish object shapes by their properties.
