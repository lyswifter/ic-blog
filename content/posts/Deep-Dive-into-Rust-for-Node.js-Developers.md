---
title: "Deep Dive Into Rust for Node"
date: 2021-06-03T18:18:48+08:00
draft: false
---

With the advent of WebAssembly (home) there has never been a better time to learn Rust on top of your existing JavaScript and Node.js knowledge for high performance computing in the browser, on the server and on the edge.

Adding Rust to your tech stack on top of Node.js is a match made in heaven as Rust provides advanced support for WebAssembly and WebAssembly binary format is runnable in Node.js.
With this deep dive, you will get up and running using Rust. By the end of this article, you will be running WebAssembly code compiled from Rust in Node.js!

Notes:
As a Node.js developer with mainly JavaScript experience, you will see unfamiliar notations like ‘ std::wx::yz ’ or ‘ &xyz’, do not worry I explain everything.

Rust is a lower-level language compared to JavaScript and Node.js. This means you are going to get familiar with how computer works to really understand what’s going on. Node.js being much higher-level, you usually don’t deal with these notions.

Remember, Rust is initially a systems programming language so closer to the metal. This gives you greater power for high performance programming but also implies more complexity.
Rust will not hide details like is the value of a variable stored on the stack or the heap, and based on that what is allowed or not. But like with Node.js, there are plenty of libraries/modules (known as crates in Rust) to make your life simple.

Again, I keep it simple.
