# Type Alias vs Interface in TypeScript: Differences and When to Use Each

## Introduction

TypeScript provides both `type` aliases and `interface` declarations to describe the shape of data. They often look similar, especially when defining object properties, but they have different capabilities. Knowing the distinction helps developers choose a clear and maintainable way to model application data.

## Detailed Explanation

An interface is primarily designed to describe object structures. It can be extended with `extends`, and declarations with the same name are merged through declaration merging.

A type alias can represent more than object shapes. It can define unions, intersections, primitives, tuples, and function types.

Both interfaces and object type aliases support many of the same object-oriented patterns. For example, an interface can extend another interface, while a type alias can combine object types with the intersection operator (`&`). However, a type alias cannot be reopened for declaration merging.

## When Should You Choose One?

Choose an interface when modelling object contracts, especially public APIs, class shapes, or structures that may be extended by other declarations. Choose a type alias when you need unions, tuples, mapped types, or a combination of different type expressions. Consistency within a project is also important.

## Conclusion

Neither option is universally better. Interfaces are convenient for extensible object contracts, while type aliases are more flexible for complex type expressions. Select the one that communicates the intended structure most clearly.
