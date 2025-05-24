---
description: >-
  This page is dedicated to giving pure in-depth explanation for every function
  and type that's defined inside of the Kauri programming language.
icon: code-simple
---

# In-Depth Explanation

## Functions

<details>

<summary><strong>print</strong></summary>

Outputs text into the CLI (Command Line Interface) and _**does not**_ end the line.\
\
**Syntax:**\
&#xNAN;**`print(text);`**\
\
**Arguments:**\
<kbd>**text**</kbd> <sup><kbd><mark style="color:orange;">R<mark style="color:orange;"><kbd></sup> Expects any [string](in-depth-explanation.md#string-str), expression, or variable. You can string together multiple `text` arguments by separating them with commas.\
\
**Examples:**\
&#xNAN;**`print("Hello", "World!");`** \
&#xNAN;**`print("Result:", 3+3);`** \
&#xNAN;**`print(x);`**

</details>

<details>

<summary><strong>println</strong></summary>

Outputs text into the CLI (Command Line Interface) and _**ends the current line.**_\
\
**Syntax:**\
&#xNAN;**`println(text);`**\
\
**Arguments:**\
<kbd>**text**</kbd> <sup><kbd><mark style="color:orange;">R<mark style="color:orange;"><kbd></sup> Expects any [string](in-depth-explanation.md#string-str), expression, or variable. You can string together multiple `text` arguments by separating them with commas.\
\
**Examples:**\
&#xNAN;**`println("Hello", "World!");`** \
&#xNAN;**`println("Result:", 3+3);`** \
&#xNAN;**`println(x);`**

</details>





## Types

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

<summary><strong>Integer</strong> <sup><kbd>int</kbd></sup></summary>

References an `integer` type. An `integer` type is any whole number, negative or positive. This is _**only**_ matched when the `integer` is isolated or not part of a `variable`.\
\
**Examples:**\
`1` \
`20` \
`300`

</details>

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

<summary><strong>Variable</strong> <sup><kbd>var</kbd></sup></summary>

References a `variable` type. A `variable` type is any string of characters staring with a letter or an underscore and ending with a letter, number, or underscore.\
\
**Examples:**\
`myVar` \
`_init_` \
`Person3`

</details>
