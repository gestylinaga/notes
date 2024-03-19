---
title: YAML
category: Data Interchange Format
---
# YAML

***WorkInProgress***

**YAML** (**Y**AML **A**in't **M**arkup **L**anguage) is a data interchange 
format, with syntax based on [Python's 🗒️](/on/python/) indentation style. 
Instead of using `{`curly braces`}` (like [JSON 🗒️](/on/json/)), or *HTML-like*
`<`tags`>` (like XML), YAML uses **whitespace** characters like indentation to 
indicate nesting. 

YAML is often used in configuration files, internet messaging, object persistence, 
and data auditing/visualization.

## Syntax
- YAML files use the file ***extensions*** `.yml` or `.yaml`
- Items are made up of **Key Value Pairs**, separated with a `:`colon, and a 
space
- **Values** can be integers, strings, arrays/lists, or objects/dictionaries
- *JSON-style* `[`brackets`]` and `{`curly braces`}` *can* be used, but are 
**not** necessary
- **List** members begin with a `-`hyphen, with 1 list item per line
- **Comments** are supported, and made with a `#`hash symbol
- `"`quotes`"` around *most* strings are **not** necessary
- For full list of **advanced** features, see the latest 
[Spec Document 🌐](https://yaml.org/spec/1.2.2/) from yaml.org

## Example
`aboutMe.yaml`
```yaml
# aboutMe.yaml -- this is a comment
first_name: Gesty
last_name: Linaga
location:
    Country: United States,
    State: California
hobbies:
    - hobby: surfing
      category: physical
    - hobby: coding
      category: creative
instrumentsIPlay: 
    - bass 
    - guitar 
    - drums...sometimes
```

## More External Links
- [YAML.org 🌐](https://yaml.org/)
- [Wikipedia Page 🌐](https://en.wikipedia.org/wiki/YAML)
