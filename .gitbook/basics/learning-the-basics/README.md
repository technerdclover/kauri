---
description: >-
  This page is dedicated to teaching anyone how the Kauri programming language
  works, ranging from basic functions to variables to data types.
icon: subtitles
---

# Learning The Basics

As a beginner, the Kauri programming language might look intimidating. There's a bunch of functions, the code might not be close to what you're familiar with, and it can be overwhelming. Luckily, this section has been handcrafted to teach you how to work with Kauri.

Firstly, you'll need to learn what some of the basic functions _are_. They'll be explained in more detail later, but for know, knowing what a function generally does is your best interest.

<table><thead><tr><th width="300.6414794921875">Function</th><th>Usage</th></tr></thead><tbody><tr><td><a data-footnote-ref href="#user-content-fn-1"><code>print</code></a>, <a data-footnote-ref href="#user-content-fn-2"><code>println</code></a></td><td>Used for printing text onto the screen.</td></tr><tr><td><a data-footnote-ref href="#user-content-fn-3"><code>prompt</code></a></td><td>Used to get the user's input.</td></tr><tr><td><a data-footnote-ref href="#user-content-fn-4"><code>let</code></a>, <a data-footnote-ref href="#user-content-fn-5"><code>const</code></a></td><td>Used to create variables.</td></tr><tr><td><code>fn</code></td><td>Used to create a function.</td></tr><tr><td><code>include</code>, <code>include as</code></td><td>Used to import Kauri Extensions (<code>.krx</code> files)</td></tr></tbody></table>

{% hint style="info" %}
Still confused? Don't worry, as some functions can be clicked on to view more information about them. This will occur in later pages as well, just in case you forget what a certain function does.
{% endhint %}

[^1]: <kbd>**print**</kbd>

    Prints text into the CLI.

    \
    **Arguments:**

    **`text`** Expects any string, expression, or variable. Can add multiple by separating with commas.

    \
    [View More](../../in-depth-explanation.md#print)

[^2]: <kbd>**println**</kbd>

    Prints text into the CLI and automatically ends the line.

    \
    **Arguments:**

    **`text`** Expects any string, expression, or variable. Can add multiple by separating with commas.



    [View More](../../in-depth-explanation.md#println)

[^3]: <kbd>**prompt**</kbd>

    Waits for the user to type something.

    \
    **Arguments:**

    `prompt` Expects a string.



    View More

[^4]: <kbd>**let**</kbd>

    Defines a mutable variable.



    **Syntax:**

    `let name: type = value;`&#x20;



    **Values:**

    `name` Any text starting with a letter and ending with a letter, number, or underscore.

    `type` Any type. Common types include `str`, `int`, `float`, `struct`, and `void`.

    `value` Any value or statement that uses the expected type.

[^5]: <kbd>**const**</kbd>&#x20;

    Defines an immutable variable.



    **Syntax:**

    `const name: type = value;`&#x20;



    **Values:**

    `name` Any text starting with a letter and ending with a letter, number, or underscore.

    `type` Any type. Common types include `str`, `int`, `float`, `struct`, and `void`.

    `value` Any value or statement that uses the expected type.
