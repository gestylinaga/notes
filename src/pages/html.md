---
layout: ../layouts/MarkdownLayout.astro
title: HTML
---

# HTML
**Hyper Text Markup Language**
```html
<!DOCTYPE html>
<html>
  <head>
    <title>This is HTML</title>
  </head>
  <body>
    <h1>This is an HTML header</h1>
  </body>
</html>
```
**Html** is a markup language that defines the structure of the content 
of a webpage. It is based on SGML (Standard Generalized Markup Language) and 
uses opening/closing tags to give organization to otherwise meaningless text: 
`<p>hi</p>`

The language underwent many changes until 2008, when it was standardized as its 
current form: **HTML5**

Some tags that HTML provides:
- `<video></video>` -- to handle video media
- `<audio></audio>` -- to handle audio media
- `<canvas></canvas>` --- to handle self-drawn graphics

HTML files contain a hierarchy of nodes based on the **DOM** 
(**D**ocument **O**bject **M**odel):
- `<html>` -- root element
- `<head>` -- element
  - `<title>` -- element
    - `"My title"` -- text
- `<body>` -- element
    - `<a>` -- element (anchor tag)
      - `href=""` -- attribute

HTML works in conjunction with CSS and JavaScript to provide complete websites.
- [see CSS](./css)
- [see JavaScript](./javascript)

## External Links
- [Official Living Standard Page](https://html.spec.whatwg.org/)
- [HTML5 - Mozilla Web Docs](https://developer.mozilla.org/en-US/docs/Glossary/HTML5)
