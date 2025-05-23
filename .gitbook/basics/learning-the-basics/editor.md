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

<pre class="language-typescript"><code class="lang-typescript">// This will retrieve the user's input without a prompt.
<strong><a data-footnote-ref href="#user-content-fn-1">prompt</a>();
</strong>
// If you want to use a prompt, then you can put a string inside of the parentheses.
<a data-footnote-ref href="#user-content-fn-1">prompt</a>("Type something: ");
</code></pre>

## Sending Output

To output something, whether it be a variable, equation, or string, you can use the [`print`](#user-content-fn-2)[^2] and [`println`](#user-content-fn-3)[^3] functions. Using [`print`](#user-content-fn-2)[^2] will print the value without a newline, while [`println`](#user-content-fn-3)[^3] will add a newline at the end.

<pre class="language-typescript"><code class="lang-typescript">// Here's some examples of print:
<a data-footnote-ref href="#user-content-fn-2">print</a>(x); // Assumes that x has a value, we'll touch on that later.
<a data-footnote-ref href="#user-content-fn-2">print</a>(3 + 3, 9 - 3);
<a data-footnote-ref href="#user-content-fn-2">print</a>("Hello, World!");

/* Result would be:
    void6Hello, World!
*/

// Using println works the same way, simply swap it out.
<a data-footnote-ref href="#user-content-fn-3">println</a>(x);
<a data-footnote-ref href="#user-content-fn-3">println</a>(3 + 3, 9 - 3);
<a data-footnote-ref href="#user-content-fn-3">println</a>("Hello, World!");

/* Result would be: 
    void
    6
    Hello, World!
*/
</code></pre>

When printing values, you can also use string interpolation, which will swap out a text segment with a variable. If the variable referenced doesn't exist, or hasn't been defined before the statement has been executed, it will replace the section with [`void`](#user-content-fn-4)[^4].

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

[^3]: <kbd>**println**</kbd>

    Prints text into the CLI and automatically ends the line.

    \
    **Arguments:**

    **`text`** Expects any string, expression, or variable. Can add multiple by separating with commas.

[^4]: <kbd>**void**</kbd>&#x20;

    Means that a value could not be found. Returning with `void` means that the code doesn't return any value.
