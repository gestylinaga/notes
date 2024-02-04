---
title: Astro
category: Web Framework
---

# Astro
**Astro** is a *fast* static site generator, based on next-gen *island
architechture*. The term "*Astro island*" refers to an interactive UI component, 
on an otherwise static page. This technique of architechtural pattern is known 
as **partial** or **selective hydration**, which lets pages load *fast*.

It has built-in support for:
- Languages:
  - [TypeScript 🗒️](/on/typescript)
  - [Markdown 🗒️](/on/markdown)
- Frameworks:
  - React
  - Svelte
  - Vue
  - Solid
- Server Side Rendering:
  - Node
  - Netlify
  - Deno

## Install
```bash
npm create astro@latest
```

## Usage
Example `.astro` file:
```astro
---
const info1 = "This area is the 'frontmatter'.";
const info2 = "TypeScript / JavaScript goes here";
---

<div>
  <h1>Plain HTML goes here</h1>
  <p>like this</p>
</div>
```

## More External Links
- [Official Site 🌐](https://astro.build/)
- [Official Docs 🌐](https://docs.astro.build/en/getting-started/)
- [GitHub Repo 🌐](https://github.com/withastro/astro)
