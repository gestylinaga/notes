---
title: JSON
category: Data Interchange Format
---
# JSON
**JSON** (**J**ava**S**cript **O**bject **N**otation) is a data interchange 
format, based on a subset of the [JavaScript 🗒️](/on/javascript/) scripting 
language 
[standard 🌐](https://ecma-international.org/publications-and-standards/standards/ecma-404/). 
Its created purpose was to be a format that was easy for humans to read and 
write, and accomplishes this by being built on two common programming 
structures:

1. A Collection of **Name/Value** Pairs -- known in most languages as an:
    - object
    - record
    - struct
    - dictionary
    - hash table
    - keyed list
    - or associative array

2. An Ordered **List** of Values -- known in most languages as:
    - array
    - vector
    - list
    - or sequence

Its use is very common across data interchange, but especially between web 
applications and servers. This means that although JSON is based on JavaScript, 
it is completely *language independent*. Many programming languages provide 
methods / libraries to generate or parse JSON-format data.

## Syntax
**Universal Syntax:**
- JSON files use the file ***extension*** `.json`
- The entire file is considered an ***object***, meaning its contents are 
wrapped in `{`curly braces`}`
- Each ***name*** is followed by a `:`colon
- Each ***name/value pair*** is separated by a `,`comma
- ***Values*** can be integers, strings, arrays, or even nested objects

**Parser Dependent:** (only available in some parsers)
- Comments are made in the [C 🗒️](/on/c/) style with `//`double slashes
- Trailing `,`commas are allowed, even on the last name/value pair

For general use, it is considered best practice to stick to universal JSON 
syntax rules to avoid parser errors or bugs.

## Example
`aboutMe.json`
```json
{
  "firstName": "Gesty",
  "lastName": "Linaga",
  "location": {
    "Country": "United States",
    "State": "California",
  },
  "hobbies": [
    { 
      "hobby": "surfing",
      "category": "physical"
    },
    {
      "hobby": "coding",
      "category": "creative"
    }
  ],
  "instrumentsIPlay": [
    "bass",
    "guitar",
    "drums...sometimes"
  ]
}
```

## More External Links
- [JSON.org 🌐](https://www.json.org/json-en.html)
- [Wikipedia Page 🌐](https://en.wikipedia.org/wiki/JSON)
