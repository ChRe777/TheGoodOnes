# GO

## Tags

- C
- Limbo, Alef
- Concurrent
- Clean

## About

Go (often referred to as Golang) is a programming language created at Google[11] in 2009 by *Robert Griesemer*, *Rob Pike*, and *Ken Thompson*.[9] Go is a statically typed compiled language in the tradition of C, with memory safety, garbage collection, structural typing,[2] and CSP-style concurrent programming features added.[12] The compiler, tools and source code are all free and open source.[13]

Go is recognizably in the tradition of C, but makes many changes to improve brevity, simplicity, and safety. The language consists of:

A syntax and environment adopting patterns more common in dynamic languages:[27]
* Optional concise variable declaration and initialization through type inference (x := 0 not int x = 0; or var x = 0;).
   * Fast compilation times.[28]
   * Remote package management (go get)[29] and online package documentation.[30]
* Distinctive approaches to particular problems:
  * Built-in concurrency primitives: light-weight processes (goroutines), channels, and the select statement.
  * An interface system in place of virtual inheritance, and type embedding instead of non-virtual inheritance.
  * A toolchain that, by default, produces **statically linked native binaries** **without external dependencies.**
  * A desire to keep the language specification simple enough to hold in a programmer's head,[31] in part by omitting features which are common in similar languages.
