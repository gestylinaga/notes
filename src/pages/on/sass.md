---
layout: ../../layouts/MarkdownLayout.astro
title: Sass
---

# Sass
**Syntactically Awesome StyleSheets**
```scss
/* This is Sass */
@mixin theme-colors($theme) {
  @if $theme == 'light' {
    background-color: $light-bg;
  } @else {
    background-color: $dark-bg;
  }
}
```
**Sass** is actually 2  compiled stylesheet languages that extend regular old
[CSS (Cascading StyleSheets)](/on/css). "Sass" refers to the compiler, 
`sass` that converts either a `.sass` or `.scss` file into a regular old `.css` 
CSS file.

### .sass 
- regular CSS without `;`s and `{}`s for *nicer / easier* syntax:
```sass 
nav
  ul
    margin: 0
    padding: 0
    list-style: none

  li 
    display: inline-block

  a 
    display: block
    padding: 6px 12px
    text-decoration: none
```

### .scss
- regular CSS with bonus features:
  - variables: 
  ```scss
  $red: hsl(0, 100%, 50%);

  .button.danger {
    color: $red;
    border: 1px solid $red;
  }
  ```
  - nesting: 
  ```scss
  .button {
    a {
      font-weight: bold;
    }

    .success {
      color: green;
    }
  }
  ```
  - mixins:
  ```scss 
  @mixin flex-column {
    display: flex;
    flex-direction: column;
    background: gray;
  }
  .card {
    @include flex-column;
  }
  .aside {
    @include flex-column;
  }
  ```
  - functions:
  ```scss 
  @mixin theme-colors($theme) {
    @if $theme == 'light' {
      background-color: $light-bg;
    } @else {
      background-color: $dark-bg;
    }
  }
  ```

## More External Links
- [Official Site](https://sass-lang.com/)
- [Official Docs](https://sass-lang.com/documentation/)
- [Official Guide](https://sass-lang.com/guide)
