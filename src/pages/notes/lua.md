---
layout: ../../layouts/MarkdownLayout.astro
title: Lua
---
# Lua
```lua 
#!/usr/bin/env lua 

local function helloWorld()
  io.write("This is Lua")
end

helloWorld()
```
**Lua** is a fast, lightweight, and embeddable scripting/programming language. 
It is widely considered the *fastest* interpreted/scripting language.

Its "virtual machine" maps very closely to the [C programming language](./c), 
and when combined with its Just-In-Time compiler, **LuaJIT**, it's faster than 
[Python](./python) and [JavaScript](./javascript).

In addition to speed, Lua's complete source code and documentation is only 
1.3 MB in size, making it very portable/embeddable.

It has seen widespread use in video-game development:
  - World of Warcraft
  - Dark Souls
  - Fable II 
  - Gary's Mod
  - Roblox

## C APIs
[Overview of C API - Lua Official Docs](http://www.lua.org/pil/24.html)

Lua's extensive C API allows easy integration, letting you call lua code in a C 
program, or vice-versa, call C code in a Lua program.

## LuaRocks
Lua has its own package manager, called **LuaRocks**.
  - [LuaRocks Official Site](https://luarocks.org/)

## External Links
- [Official Site](https://www.lua.org/)
- [Official Docs](https://www.lua.org/docs.html)
- [Official Reference Manual 5.1](https://www.lua.org/manual/5.1/)
- [The LuaJIT Project](https://luajit.org/)
