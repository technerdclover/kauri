---
description: >-
  Input and output in Kauri is simple. In this section, we’ll go over input and
  output, as well as a few ways that they can be used.
icon: input-text
---

# Basic I/O

{% hint style="info" %}
Note: Syntax highlighting might be inconsistent.
{% endhint %}

## Getting Input

To get an input, you can use the [`prompt`](#user-content-fn-1)[^1] function. This function can be used with and without a prompt specified, though it is recommended to use a prompt when asking for an input.

```typescript
// This will retrieve the user's input without a prompt.
prompt();

// If you want to use a prompt, then you can put a string inside of the parentheses.
prompt("Type something: ");
```

## Sending Output

To output something, whether it be a variable, equation, or string, you can use the [`print`](#user-content-fn-2)[^2] and [`println`](#user-content-fn-3)[^3] functions. Using [`print`](#user-content-fn-4)[^4] will print the value without a newline, while [`println`](#user-content-fn-3)[^3] will add a newline at the end.

<pre class="language-typescript"><code class="lang-typescript">// Here's some examples of <a data-footnote-ref href="#user-content-fn-4">print</a>:
print(x); // Assumes that x has a value, we'll touch on that later.
print(3 + 3, 9 - 3);
print("Hello, World!");

/* Result would be:
    void6Hello, World!
*/

// Using <a data-footnote-ref href="#user-content-fn-3">println</a> works the same way, simply swap it out.
println(x);
println(3 + 3, 9 - 3);
println("Hello, World!");

/* Result would be: 
    void
    6
    Hello, World!
*/
</code></pre>

When printing values, you can also use string interpolation, which will swap out a text segment with a variable. If the variable referenced doesn't exist, or hasn't been defined before the statement has been executed, it will replace the section with [`void`](#user-content-fn-5)[^5].

```typescript
// This will print the value of the "score" variable along with some text.
println("The score value is: <$score>");
```



[^1]: <kbd>**prompt**</kbd>

    Waits for the user to type something.

    \
    **Arguments:**

    `prompt` Expects a string.

[^2]: <kbd>**print**</kbd>

    Prints text into the CLI.

    \
    **Arguments:**

    **`text`** Expects any string, expression, or variable. Can add multiple by separating with commas.



    <a href="../../in-depth-explanation.md#print" class="button secondary">View More</a>

[^3]: <kbd>**println**</kbd>

    Prints text into the CLI and automatically ends the line.

    \
    **Arguments:**

    **`text`** Expects any string, expression, or variable. Can add multiple by separating with commas.

[^4]: <kbd>**print**</kbd>

    Prints text into the CLI.

    \
    **Arguments:**

    **`text`** Expects any string, expression, or variable. Can add multiple by separating with commas.

[^5]: <kbd>**void**</kbd>&#x20;

    Means that a value could not be found. Returning with `void` means that the code doesn't return any value.
