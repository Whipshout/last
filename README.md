# Rust binary integration in Javascript

## Contact
- Eduardo Sánchez<br>


- whipshout@gmail.com<br>


- https://www.linkedin.com/in/eduardo-sanchez-sanchez/ <br>

## Info

- We can integrate **Rust with Node through native addons**, as we would with **C++**. <br>


- To do this, we have to interact with **Javascript through C**. We compile a **Rust library using C interfaces and bindings**. The library is in different formats depending on the operating system.<br>


- To do all the hard work, we use the **crate called NAPI**, which is responsible for making the interfaces and bindings with C and exporting the functions for use in Javascript.

## NAPI crate

- **NAPI** => https://napi.rs/ <br>


- **NAPI Crate** => https://crates.io/crates/napi <br>


- **NAPI GitHub** => https://github.com/napi-rs/napi-rs <br>


- **NAPI Examples** => https://github.com/napi-rs/napi-rs/tree/main/examples <br>

## How to use the native addon

- Create/open a javascript/typescript project.<br>


- Install the package using ```npm install wtools-rust```. The main package will install the right dependency for your OS automatically.<br>


- Import the package and call the function (Typescript snippet, functions have ts types generated during the compilation):
```
import { uuid } from "./index";

const uuidRandom = uuid() // Generate random uuid

const uuidInput = uuid('asdfadfsadsf') // Generate uuid using hash SHA256 with the input text
```

