---
description: >-
  Types are simple in Kauri. In this section, we'll go over basic types, as well
  as some basic math.
icon: kerning
---

# Basic Types & Math

{% hint style="info" %}
Note: Syntax highlighting might be inconsistent.
{% endhint %}

## Understanding Types

There's a variety of different types in Kauri. This helps to organize everything, as well as clearly define how things should work. Types are important, as they allow the code to understand what type of value something is. If a variable has a string type, then it should be treated as a line of text and not a number.

Below is a list of different types, including an example of what they are and how they are defined.

<table><thead><tr><th width="125.83013916015625">Type</th><th width="269.37738037109375">Explanation</th><th>Example</th></tr></thead><tbody><tr><td><a data-footnote-ref href="#user-content-fn-1">int</a></td><td>Used to define a whole number.</td><td><code>3, 6, 9, 12</code></td></tr><tr><td><a data-footnote-ref href="#user-content-fn-2">float</a></td><td>Used to define a decimal number.</td><td><code>3.14, 6.28, 9.99</code></td></tr><tr><td><a data-footnote-ref href="#user-content-fn-3">string</a></td><td>Used to define a line of text.</td><td><code>"Hello, World!"</code></td></tr><tr><td><a data-footnote-ref href="#user-content-fn-4">struct</a></td><td>Used to define a structure.</td><td><code>{ name: str; age: int; }</code></td></tr><tr><td><a data-footnote-ref href="#user-content-fn-5">void</a></td><td>Used to indicate a lack of value.</td><td><code>void</code></td></tr></tbody></table>

\
\
\
\
\
\
\
\


[^1]: <kbd>**Int**</kbd>

    Used to define any whole number.



    **Example:**

    `1000, 50, 92`



    [Learn More](../../in-depth-explanation.md#integer-int)

[^2]: <kbd>**Float**</kbd>

    Used to define any decimal number.



    **Example:**

    `3.14159, 6.28318, 9.99`



    [Learn More](../../in-depth-explanation.md#float-float)

[^3]: <kbd>**String**</kbd>

    Used to define a string of text surrounded by double quotes.



    **Example:**

    `"Hello, World!"`



    [Learn More](../../in-depth-explanation.md#string-str)

[^4]: <kbd>**Struct**</kbd>

    Used to define a structure that can be used by a [`type`](../../in-depth-explanation.md#type) function.



    **Example:**

    `{ name: str; age: int; }`



    [Learn More](../../in-depth-explanation.md#struct-struct)

[^5]: <kbd>**Void**</kbd>

    Used to indicate a lack of value or an undefined value.



    **Example:**

    `void`



    [Learn More](../../in-depth-explanation.md#void-void)
