# Classes, Inheritance, Functional Programming

## Research Questions:

**1. Why would you want to run JavaScript code outside of a browser?**

Running JavaScript without/outside a browser means you are using node.js technology to execute your JavaScript code. This type of usage of javascript typically refers to backend programming where your javascript code will interact with your database and can be used to create RESTful APIs.

**2. What is the difference between a module and a package?**

Modules are libraries for Node.js.

Node.js has a simple module loading system. In Node.js, files and modules are in one-to-one correspondence.

Examples of modules:

- Circle.js
- Rectangle.js
- Square.js

**A package is one or more modules (libraries) grouped (or packaged) together. These are commonly used by other packages or a project of your own. Node.js uses a package manager, where you can find and install thousands of packages.**

Example of a package:

Shapes             <- Package name
  - Circle.js      <-
  - Rectangle.js   <- Modules that belong to the Shapes package
  - Square.js      <-

**Essentially, you could install the package, Shapes, and have access to the Circle, Rectangle, and Square modules.**

**3. What does the node package manager do?**

Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node.js packages in your application. It is also an online repository for open-source Node.js packages.

**4. Provide code snippets showing 3 different ways to export a function from a node module**

1. Export Function as a Class :
In JavaScript, a function can be treated like a class. The following example exposes a function that can be used like a class.
```
module.exports = function (firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.fullName = function () { 
        return this.firstName + ' ' + this.lastName;
    }
}
```

2. Export the function using `module.exports.` :

```
module.exports = function (a, b) { 
  console.log(a + b); 
} 
```


## Vocabulary Terms :

- ecosystem : The simplest definition of an ecosystem is that it is a community or group of organisms that live in and interact with each other in a specific environment.

- Node.js : Node.js is an open-source, cross-platform, JavaScript runtime environment that executes JavaScript code outside a web browser.

- V8 Engine : V8 is Google’s open source high-performance JavaScript and WebAssembly engine, written in C++. It is used in Chrome and in Node.js, among others. It implements ECMAScript and WebAssembly, and runs on Windows 7 or later, macOS 10.12+, and Linux systems that use x64, IA-32, ARM, or MIPS processors. V8 can run standalone, or can be embedded into any C++ application.

- module : Module in Node.js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node.js application.

- package : package is one or more modules (libraries) grouped (or packaged) together. These are commonly used by other packages or a project of your own. Node.js uses a package manager, where you can find and install thousands of packages.

- node package manager (npm) : Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node.js packages in your application. It is also an online repository for open-source Node.js packages.

- server : server is a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients". This architecture is called the client–server model. Servers can provide various functionalities, often called "services", such as sharing data or resources among multiple clients, or performing computation for a client

- environment : is a workspace for developers to make changes without breaking anything in a live environment. An integrated development environment is often used as a programming tool to assist the developer. An integrated development environment (IDE) is the software suite used by developers and is designed to maximize productivity and efficiency for the developer.

- interpreter : Interpreter is a program that executes instructions written in a high-level language. There are two ways to run programs written in a high-level language. The most common is to compile the program; the other method is to pass the program through an interpreter. An interpreter translates high-level instructions into an intermediate form, which it then executes. In contrast, a compiler translates high-level instructions directly into machine language

- compiler : is a computer program that translates computer code written in one programming language (the source language) into another language (the target language).