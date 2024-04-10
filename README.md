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
print("Hello World!")
```

> Note: A string will always be enclosed be quotation marks

We are also not limited to the number of print statements we can have

For example:

```lua
print("Hello World !")
print("My name is AGNEAY B NAIR")
```

To print multiple  text using the same print statement we can use of the below given format

Format:

```lua
print("HELLO WORLD","I LOVE LUA")
```

the above print statement will display the two strings together by seperating them by a `tab` space

inorder to concatenate two strings using the `print` statement in lua use `..` instead of `, ` in the print statement

For example:

```lua
print("Hello world!".." I love lua !")
```

will concatenate both the strings

## Variables and data types:

- The undefined data types: The `nil` data type is undefined and empty

- The number data type: `number`

- `string` data type : all characters enclosed within quotes

- `boolean` data type: `true` and `false`

- `tables` data type: The equivalent of array or list present in different programming languages
  
  ## To create a local variable
  
  ```lua
  local name
  ```

   here `name` is the variable name

lua always explicitly places the nil data type to the variable . Hard to believe ? Let's try it out

```lua
local name
print(name)
```

This would return nil as the variable name stores nil

we can also implicitly give `name` the value nil as

For example:

```lua
local name = nil
print(name)
```

It is not necessary to define the value in the same line as that in which we define the variable

```lua
local name
name = nil
print(name)
```

we can also use print statement to display  the value of expressions

For example:

```lua
local x = 3
print(x+8)
```

## To define a global variable

```lua
GlobalVar = 3
```

Here the variable `GlobalVar` has the value 3 and is globally defined and can be imported in other lua files

inorder to define a global variable to lua more spefically to lua we could write

```lua
_G.GloablVar = 3
```

Here the prefix _G. will make it clear to lua that we intend to create a global variable and not a local variable

> NOTE: we need not use _G. always it is completly optional 

## To define multiple local variable at the same time

```lua
local name,age,gender
```

now we have defined three variables at the same time

we could also give them values as we define them as

```lua
local namea,nameb,namec = "ram","lak","shah"
```

here we have created three variable having same data type , but this is not a necessesity ie we can define variables having different data type in the same line

```lua
local name,age,gender = "AGNEAY",18,"MALE"
```

## Getting the length of the string

we can get the length of any string in lua with the help of `#`

For example:

```lua
local x = "AGNEAY B NAIR"
print(#x)
```

The above code will return the length of string, we can also do it this way

```lua
local x = #"AGNEAY B NAIR"
print(x)
```

## To check the type of a given data type

we can simply use `type()` function provided by lua

For example:

```lua
local x = "AGNEAY B NAIR"
local y = 13
local z = true
print(type(x),type(y),type(z))
```

## To convert a number to string:

we can use the `tostring()` function provided by lua

```lua
local x = 18
print(type(x))
local y = tostring(x)
print(type(y)
```

## Escape sequence

| Escape sequence | meaning           |
|:---------------:|:-----------------:|
| \n              | newline character |
| \t              | tab space         |
| \\\             | \                 |

