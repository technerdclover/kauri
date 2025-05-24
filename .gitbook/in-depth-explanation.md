---
description: >-
  This page is dedicated to giving pure in-depth explanation for every function
  and type that's defined inside of the Kauri programming language. Any argument
  with Req or Opt means Required or Optional.
icon: code-simple
---

# In-Depth Explanation

## Functions

<details>

<summary><strong>const</strong></summary>

<sub>_**Non-returning Function**_</sub>\
Creates an immutable variable, meaning it _**can't be**_ overwritten.\
\
**Syntax:**\
&#xNAN;**`const variable: type = value;`**\
\
**Arguments:**\
<kbd>**variable**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any [Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var). You cannot use periods when defining this variable.\
\
<kbd>**type**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any _**non**_-[Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var) [Type](in-depth-explanation.md#types). Must be a pre-defined type.\
\
<kbd>**value**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any [Type](in-depth-explanation.md#types) or Returning [Function](in-depth-explanation.md#functions) (such as [prompt](in-depth-explanation.md#prompt)). You cannot loop `let` or `const` statements inside of the value.\
\
**Examples:**\
`const x: int = 5;` \
`const name: str = prompt("Type your name: ");` \
`const tau: float = math.pi * 2;`

</details>

<details>

<summary><strong>let</strong></summary>

<sub>_**Non-returning Function**_</sub>\
Creates a mutable variable, meaning it _**can be**_ overwritten.\
\
**Syntax:**\
&#xNAN;**`let variable: type = value;`**\
\
**Arguments:**\
<kbd>**variable**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any [Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var). You cannot use periods when defining this variable.\
\
<kbd>**type**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any _**non**_-[Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var) [Type](in-depth-explanation.md#types). Must be a pre-defined type.\
\
<kbd>**value**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any [Type](in-depth-explanation.md#types) or Returning [Function](in-depth-explanation.md#functions) (such as [prompt](in-depth-explanation.md#prompt)). You cannot loop `let` or `const` statements inside of the value.\
\
**Examples:**\
`let x: int = 5;` \
`let name: str = prompt("Type your name: ");` \
`let tau: float = math.pi * 2;`

</details>

<details>

<summary><strong>print</strong></summary>

<sub>_**Non-returning Function**_</sub>\
Outputs text into the CLI (Command Line Interface) and _**does not**_ end the line.\
\
**Syntax:**\
&#xNAN;**`print(text);`**\
\
**Arguments:**\
<kbd>**text**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any [String <sup><kbd>str<kbd></sup>](in-depth-explanation.md#string-str), expression, or [Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var). You can string together multiple `text` arguments by separating them with commas.\
\
**Examples:**\
`print("Hello", "World!");` \
`print("Result:", 3+3);` \
`print(x);`

</details>

<details>

<summary><strong>println</strong></summary>

<sub>_**Non-returning Function**_</sub>\
Outputs text into the CLI (Command Line Interface) and _**ends the current line.**_\
\
**Syntax:**\
&#xNAN;**`println(text);`**\
\
**Arguments:**\
<kbd>**text**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any [String <sup><kbd>str<kbd></sup>](in-depth-explanation.md#string-str), expression, or [Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var). You can string together multiple `text` arguments by separating them with commas.\
\
**Examples:**\
`println("Hello", "World!");` \
`println("Result:", 3+3);` \
`println(x);`

</details>

<details>

<summary><strong>prompt</strong></summary>

<sub>_**Returning Function**_</sub>\
Waits for an input from the user and returns their input.\
\
**Syntax:**\
&#xNAN;**`prompt(text);`**\
\
**Arguments:**\
<kbd>**text**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any [String <sup><kbd>str<kbd></sup>](in-depth-explanation.md#string-str), expression, or [Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var). You can string together multiple `text` arguments by separating them with commas.\
\
**Examples:**\
`prompt("Type", "Something: ");` \
`prompt("ID", name);` \
`prompt(x);`

</details>

<details>

<summary><strong>type</strong></summary>

<sub>_**Non-returning Function**_</sub>\
Creates a [Type](in-depth-explanation.md#types) that can be used when defining variables.\
\
**Syntax:**\
`type variable: type = value;`

\
**Arguments:**\
<kbd>**variable**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any [Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var). You cannot use periods when defining this variable.\
\
<kbd>**type**</kbd> <sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects any _**non**_-[Variable <sup><kbd>var<kbd></sup>](in-depth-explanation.md#variable-var) [Type](in-depth-explanation.md#types). Must be a pre-defined type.\
\
<kbd>**value**</kbd> <sup><kbd><mark style="color:blue;">Opt<mark style="color:blue;"><kbd></sup><sup><kbd>/<kbd></sup><sup><kbd><mark style="color:green;">Req<mark style="color:green;"><kbd></sup> Expects a default value for the type. If the `type` argument is set to a [Struct <sup><kbd>struct<kbd></sup>](in-depth-explanation.md#struct-struct), the value should be formatted as `{ value: type; value: type; }`. _**Only required**_ if the `type` argument is set to a [Struct <sup><kbd>struct<kbd></sup>](in-depth-explanation.md#struct-struct).

\
**Examples:**\
`type Login: struct = { name: str; pass: str; };`\
`type ID: int = void;` \
`type Passwd: str;`

</details>



## Types

<details>

<summary><strong>Float</strong> <sup><kbd>float</kbd></sup></summary>

References a `float` type. A `float` type is any decimal number, negative or positive. This is _**only**_ matched when the `float` is isolated or not part of a `variable`.\
\
**Examples:**\
`3.14159` \
`6.28318` \
`50.3`

</details>

<details>

<summary><strong>Integer</strong> <sup><kbd>int</kbd></sup></summary>

References an `integer` type. An `integer` type is any whole number, negative or positive. This is _**only**_ matched when the `integer` is isolated or not part of a `variable`.\
\
**Examples:**\
`1` \
`20` \
`300`

</details>

<details>

<summary><strong>String</strong> <sup><kbd>str</kbd></sup></summary>

References a `string` type. A `string` type starts and ends with a double-quote (`"`). It matches the closest double-quote, meaning that it will only match until the next double-quote is found.\
\
**Examples:**\
`"Hello, World!"` \
`"This is a string!"` \
`"Score: <$score>"`

</details>

<details>

<summary><strong>Struct</strong> <sup><kbd>struct</kbd></sup></summary>

References a `struct` type. A `struct` type starts and ends with enclosing curled-brackets (`{` and `}`). Inside of the struct, values will be formatted as `value: type;` and can be accessed via string interpolation by doing `<$StructName.value>`.\
\
**Examples:**\
`{ ID: int; }` \
`{ User: str; Pass: str; }` \
`{ Health: int; Strength: int; Level: float; }`

</details>

<details>

<summary><strong>Variable</strong> <sup><kbd>var</kbd></sup></summary>

References a `variable` type. A `variable` type is any string of characters staring with a letter or an underscore and ending with a letter, number, or underscore.\
\
**Examples:**\
`myVar` \
`_init_` \
`Person3`

</details>

<details>

<summary><strong>Void</strong> <sup><kbd>void</kbd></sup></summary>

References a `void` type. A `void` type either means that a value doesn't exist (getting `void` when using string interpolation) or a function doesn't return anything (if used as a return type in a function).

</details>

