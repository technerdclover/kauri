---
description: >-
  Input and output in Kauri is simple. In this section, we’ll go over input and
  output, as well as all of the various ways that they can be used.
icon: block-quote
---

# Variable Assignment

## Basic Variable Assignment

Making variables is simple with Kauri. You can make mutable or immutable variables, which define whether or not they can be modified after creation. To make a variable, check the code below.

```typescript
// Using let will create mutable variables, which can be changed later.
let five: int = 5;
let pi: float = 3.14159;
let prompt: str = "Hello, World! Type something: ";

// Using const works the same way, but these can't be changed later.
const six: int = 6;
const tau: float = 6.28319;
const random: str = "Hello, World! You can't change this!";
```

As mentioned in the code comments, you can override variables that are mutable. It’s easy to do this, and all it requires is redefining the variable with either [`const`](#user-content-fn-1)[^1] or [`let`](#user-content-fn-2)[^2] statements.

```typescript
// Here we'll define a variable called "x" and then override it with let.
let x: int = 5;
let x: int = 8;

// Here we'll do the same thing, this time using const.
let x: int = 5;
const x: int = 8;
```

{% hint style="info" %}
As of the latest release, you can also override constant variables with another constant variable. Here's an example.

```typescript
const x: int = 5; // x is set to 5
const x: int = 8; // x is now set to 8
```
{% endhint %}

[^1]: <kbd>**const**</kbd>&#x20;

    Defines an immutable variable.



    **Syntax:**

    `const name: type = value;`&#x20;



    **Values:**

    `name` Any text starting with a letter and ending with a letter, number, or underscore.

    `type` Any type. Expects `str`, `int`, `float`, `struct`, or `void`.

    `value` Any value or statement that uses the expected type.

[^2]: <kbd>**let**</kbd>

    Defines a mutable variable.



    **Syntax:**

    `let name: type = value;`&#x20;



    **Values:**

    `name` Any text starting with a letter and ending with a letter, number, or underscore.

    `type` Any type. Expects `str`, `int`, `float`, `struct`, or `void`.

    `value` Any value or statement that uses the expected type.
