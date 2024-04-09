# Welcome to Lua-Cheatsheet

---

---

## Comments :

---

Comments in lua are of two types:

- single line comment

- multi line comment

### single line comment:

A single line comment in lua is given by adding `--` to the begining of the line

For example:

```lua
-- This is a comment
```

It is not necessary to leave a space after `--` to the make a comment

For example:

```lua
--This is also a comment
```

Lua also does not restrict the number of comments possible for example

```lua
-- this is comment 1
-- this is comment 2
-- this is comment 3
```

### multi line comment :

A  multiline comment is lua begins with `--[[` and ends with `]]`

For example:

```lua
--[[
    This 
    is 
    a 
    multiline
    comment
]]
```

> Make sure there is no space between `--` and `[[` in the start of the multiline comment as doing so will cause `Error`

> NOTE: Comments can be place wherever we want for example they can be placed after a meaningful statements 
> 
> For example:
> 
> ```lua
> print("Hello World!") -- This statement will be ignored
> ```

## Printing stuffs onto screen:

In lua we can print

- texts

- variables

### printing texts onto screen:

To print text onto screen we need to simply use the print statement in the following format is `print(<text to be printed>)`

For example:

```lua
print("Hello World!")
```

> Note: A string will always be enclosed be quotation marks

We are also not limited to the number of print statements we can have

For example:

```lua
print("Hello World !")
print("My name is AGNEAY B NAIR")
```


