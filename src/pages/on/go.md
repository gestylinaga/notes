---
layout: ../../layouts/MarkdownLayout.astro
title: Go
---

# Go
```go
package main

import "fmt"

func main() {
  fmt.Println("This is Go")
}
```
**Go** (or **Golang**) is a statically typed, compiled language often described 
as [C](/on/c) for the 21st century. It is a popular choice for high-performance 
server-side applications. 

It has built tools like:
  - Docker
  - CockroachDB
  - Dgraph

It was built in 2007 at Google, by Ken Thompson (who also created the B, and C 
programming languages). Go was designed for simplicity and efficiency, with 
version 1.0 realeasing in 2012 as open-source software.

Go is famous for its *extremely* fast compile times, which is made possible with
its innovations on dependancy analysis.

Even though it is a *statically* typed language, it performs type inference to 
provide a very clean / concise syntax.

The language also allows you to store the memory address of a value to a 
pointer, while disallowing pointer arithmetic (which often leads to 
undpredictable behavior).

Additionally, Go supports **concurrency** with '*Go Routines*', which are 
functions that can run at the same time as other functions by utilizing multiple
threads on a CPU.

## Go Modules
Go has its own package / module system, making it easy to import or export code 
between projects. Running `go mod init` in a terminal, creates a go module file
(`go.mod`) that enables dependancy tracking (just like a `package.json` in 
[JavaScript](/on/javascript)).

## More External Links
- [Official Site](https://go.dev/)
- [Official Docs](https://go.dev/doc/)
- [Go page on Wikipedia](https://en.wikipedia.org/wiki/Go_(programming_language))
