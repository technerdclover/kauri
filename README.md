# Kauri
When programming feels natural.

---

The Kauri programming language is designed for creating CLI (Command Line Interface) tools and applications. It takes features from C++, TypeScript, and Python and offers clear and natural syntax akin to other programming languages. This allows the language to have easily readable code, even for developers who don't use Kauri.

Kauri is built on Python, which means that it will take a hit performance-wise, but otherwise allows for easy debugging and the addition of new functions. Below is an example of a Kauri script, using the `.kri` extension.
```kauri
type Person: struct = {
  name: str;
  age: int;
};

let jackie: Person = {
  "Jackie",
  age: 19
};

println("Name: <$jackie.name>");
println("Age: <$jackie.age>");
```
```
Name: Jackie
Age: 19
```

To read the documentation for Kauri, click on [this link](https://kauri-language.gitbook.io/kauri/).
