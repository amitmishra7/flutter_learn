# Dart Basics

<img src="https://swansoftwaresolutions.com/wp-content/uploads/2020/02/08.20.20-What-is-Dart-and-how-is-it-used-1024x576.jpg" height=400/>

### Table of Contents
**[What is Dart?](#what-is-dart)**<br>
**[Dart: Uses](#dart-uses)**<br>
**[Dart: Objectives](#dart-objectives)**<br>
**[Dart: Why?](#dart-why)**<br>
**[Dart: The language](#dart-the-language)**<br>
**[Dart: The libraries](#dart-the-libraries)**<br>
**[Dart: The platforms](#dart-the-platform)**<br>
    **[Dart Native (machine code JIT and AOT)](#dart-native)**<br>
    **[Dart Web (JavaScript dev & prod)](#dart-web)**<br>
    **[Dart runtime](#dart-runtime)**<br>
**[Dartpad](#dartpad)**<br>

## What is Dart?

Dart is a client-optimized language for developing fast apps on any platform. Its goal is to offer the most productive programming language for multi-platform development, paired with a flexible execution runtime platform for app frameworks.

The Dart programming language was first launched back in 2011 at a conference in Denmark. At that time, the Dart language was relatively small compared to other languages such as C#, JavaScript, or Python. But this changed with the release of Flutter.

## Dart: Uses

Dart is used with Flutter to build mobile apps. This is one of the most common uses of Dart today. The big benefit of building apps with Dart and Flutter is that it is cross-platform. It means that you can build an app with just one code base instead of building two separate apps for iPhone and Android. 

Dart is not limited to building the frontend for Flutter apps. You can use it on the backend as a server-side programming language too. But it is far from as popular as other server-side languages such as PHP, Node or Python. It is probably not the best choice for a backend today because it has a small community. This means you have to build everything from scratch.

## Dart: Objectives

According to the official documentation, Dart is a long-term project with ambitious objectives. The core objectives are:
Dart has a strong support base with many libraries and tools, which enable very large applications.
One of the major objectives of Dart is to simplify programming tasks. It is designed to make common programming tasks simpler.
Dart is very stable and it can be used to build real-time applications with production quality. It is an object-oriented programming language with support for inheritance, interfaces and optional typing features.

## Dart: Why?

Dart is an oop language so, you can think where Java is you can see the Dart. Right now you can see the trends of the Flutter App Development. Flutter fully depends on the Dart and through the Dart, you can build mobile, desktop, server, and web applications. So, this is the plus for you to go for the dart language. When you OOP programming you can easily switch to other programming languages as well.


## Dart: The language

The Dart language is type safe; it uses static type checking to ensure that a variable’s value always matches the variable’s static type. Sometimes, this is referred to as sound typing. Although types are mandatory, type annotations are optional because of type inference. The Dart typing system is also flexible, allowing the use of a dynamic type combined with runtime checks, which can be useful during experimentation or for code that needs to be especially dynamic.

```
void main() {
  print('Hello, World!');
}
```

## Dart: The libraries

Dart has a rich set of core libraries, providing essentials for many everyday programming tasks:

* Built-in types, collections, and other core functionality for every Dart program (dart:core)
* Richer collection types such as queues, linked lists, hashmaps, and binary trees (dart:collection)
* Encoders and decoders for converting between different data representations, including JSON and UTF-8 (dart:convert)
* Mathematical constants and functions, and random number generation (dart:math)
* File, socket, HTTP, and other I/O support for non-web applications (dart:io)
* Support for asynchronous programming, with classes such as Future and Stream (dart:async)
* Lists that efficiently handle fixed-sized data (for example, unsigned 8-byte integers) and SIMD numeric types (dart:typed_data)
* Foreign function interfaces for interoperability with other code that presents a C-style interface (dart:ffi)
* Concurrent programming using isolates—independent workers that are similar to threads but don’t share memory, communicating only through messages (dart:isolate)
* HTML elements and other resources for web-based applications that need to interact with the browser and the Document Object Model (DOM) (dart:html)

## Dart: The platforms

Dart’s compiler technology lets you run code in different ways:

* `Native platform`: For apps targeting mobile and desktop devices, Dart includes both a Dart VM with just-in-time (JIT) compilation and an ahead-of-time (AOT) compiler for producing machine code.

* `Web platform`: For apps targeting the web, Dart can compile for development or production purposes. Its web compiler translates Dart into JavaScript.

<img src="https://dart.dev/assets/img/Dart-platforms.svg" height=400/>

### Dart Native (machine code JIT and AOT)

During development, a fast developer cycle is critical for iteration. The Dart VM offers a just-in-time compiler (JIT) with incremental recompilation (enabling hot reload), live metrics collections (powering DevTools), and rich debugging support.

When apps are ready to be deployed to production—whether you’re publishing to an app store or deploying to a production backend—the Dart ahead-of-time (AOT) compiler can compile to native ARM or x64 machine code. Your AOT-compiled app launches with consistent, short startup time.

The AOT-compiled code runs inside an efficient Dart runtime that enforces the sound Dart type system and manages memory using fast object allocation and a generational garbage collector.

### Dart Web (JavaScript dev & prod)

Dart Web enables running Dart code on web platforms powered by JavaScript. With Dart Web, you compile Dart code to JavaScript code, which in turn runs in a browser—for example, V8 inside Chrome.

Dart web contains two compiliation modes:

An incremental development compiler enabling a fast developer cycle
An optimizing production compiler which compiles Dart code to fast, compact, deployable JavaScript. These effeciencies come from techniques such as dead-code elimination.

### Dart runtime

Regardless of which platform you use or how you compile your code, executing the code requires a Dart runtime. This runtime is responsible for the following critical tasks:

Managing memory: Dart uses a managed memory model, where unused memory is reclaimed by a garbage collector (GC).

Enforcing the Dart type system: Although most type checks in Dart are static (compile-time), some type checks are dynamic (runtime). For example, the Dart runtime enforces dynamic checks by type check and cast operators.

Managing isolates: The Dart runtime controls the main isolate (where code normally runs) and any other isolates that the app creates.

On native platforms, the Dart runtime is automatically included inside self-contained executables, and is part of the Dart VM provided by the dart run command.


## Dartpad

DartPad is an open source tool that lets you play with the Dart language in any modern browser. Many pages in this site—especially codelabs—have embedded DartPads. To open DartPad as a standalone web page, visit the DartPad site [(dartpad.dev)](https://dartpad.dev/)





