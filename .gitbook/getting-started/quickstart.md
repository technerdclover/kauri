---
description: >-
  This page provides an overview of the Kauri programming language, including
  instructions on how to install it and compile it from scratch.
icon: bullseye-pointer
---

# Quickstart

### Overview

The Kauri programming language is designed for creating CLI (Command Line Interface) tools and applications. It takes features from C++, TypeScript, and Python and offers clear and efficient syntax. This allows the language to have easily readable code, even for developers who don't use Kauri.

{% hint style="info" %}
Want to explore the syntax? Head to the [Basics](../basics/learning-the-basics/editor.md) section to learn more.
{% endhint %}

### Installation

Kauri offers two installation methods: download a pre-compiled version suitable for your operating system or compile it using the source files.

{% tabs %}
{% tab title="Pre-Compiled" %}
To install a pre-compiled version of Kauri:

1. Download the latest release.
   * Locate the [Releases](https://github.com/technerdclover/kauri/releases) page for the Kauri language on GitHub.
   * Locate the build for your OS and download the executable.
2. Add the executable to your system's PATH.
{% endtab %}

{% tab title="Source Build" %}
To compile Kauri's source code from scratch:

1. Ensure that `python3` and `pip` are both installed.
2. Download a python compiler using `pip` (such as `nuitka` or `pyinstaller`)
3. Download the latest release.
   * Locate the [Releases](https://github.com/technerdclover/kauri/releases) page for the Kauri language on GitHub.
   * Locate the source code file and download it.
   * Alternatively, you can use `git clone https://github.com/technerdclover/kauri`.
4. Use the compiler to compile Kauri's source code into one executable.
5. Add the newly created executable to your system's PATH.
{% endtab %}
{% endtabs %}

{% hint style="info" %}
Don't know how to access your PATH? Check here:

* Linux:
  * Open a terminal window
  * Type "nano ./bashrc" and press Enter. (Do "nano ./zshrc" if using zsh.)
  * Add a line at the bottom and type "export PATH=$PATH:/path/to/kauri" (replace "/path/to/kauri" with the actual directory)
  * Press Ctrl + S and Ctrl + X to save and exit.
* Windows:
  * Press Windows + R
  * Type "sysdm.cpl" and press Enter.
  * Go to Advanced > Environment Variables
  * In system variables, find a variable called "Path"
  * Hit enter and press the New button, then type the directory where Kauri is stored.
{% endhint %}
