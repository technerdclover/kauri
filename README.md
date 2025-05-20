# Kauri
A simplistic programming language.

---

Kauri, otherwise known as the Kauri Programming Language, is a programming language designed to be simplistic and fresh compared to most other programming languages. It uses elements from a variety of programming languages, including (but not limited to) C++, Javascript, and Python.

Kauri is built on Python, which means that it will take a hit performance-wise, but otherwise allows for easy debugging and the addition of new functions. Below is an example of a Kauri script, using the `.kri` extension.
```kauri
type Person: struct = {
  name: str
  age: int
}

let jackie: Person = {
  "Jackie",
  19
}

println("Name: <$jackie.name>");
println("Age: <$jackie.age>");
```
```
Name: Jackie
Age: 19
```

To read the documentation for Kauri, click on [this link]().
