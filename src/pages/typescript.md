---
layout: ../layouts/MarkdownLayout.astro
title: TypeScript
---

# TypeScript
```typescript
let someString: string = "This is TypeScript";
let someNumber: number = 324;
let someBool: boolean;

function helloWorld() {
  console.log(someString);
}

helloWorld()
```
**TypeScript** is a *strongly typed* programming language that builds 
on [JavaScript](../javascript). It is a strict superset of JavaScript, 
meaning that you can write plain JavaScript in a `.ts` file, and the extra 
features of TypeScript are completely optional. This is because TypeScript acts 
like a compiled language, that eventually compiles into regular old JavaScript.

## Advantages
- Strong static typing
- Error checking before runtime
- Practically no learning curve if you know JavaScript
- Compile into any version of JavaScript (for browser backwards compatability)

## External Links
- [Official Site](https://www.typescriptlang.org/)
- [Official Docs](https://www.typescriptlang.org/docs/)
- [Official Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)
