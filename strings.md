
Strings are everywhere. Anything that’s in quotes, is a string. So that means...

```other
"This is a string."
'So is this'
"But did you know that... ".. " this is all one string? (Sort of)"

-- Whenever you do....
print("this,")

-- You're using a string!
Whenever you do....
script.Parent.Name = "New name"
-- You're using a string!
```

So yeah, strings are used everywhere. But what are some more advanced things we can do with them?

---

## Concatenation

Concatenation is when you combine a string with another string or number. For example, this is  all one string.

```other
local myepicstring = "Hello ".. "world!"
print(myepicstring)

-- This will print out "Hello world"
```

Any two strings can be combined using two dots after the first string and then a space.

`”Like”.. “this”`

You can also use this method with variables.

```other
local stringone = "Hello " -- Combining two strings won't automatically add a space. If you want it, make sure that one of the two strings starts or ends in a space.
local stringtwo = "world"

print(stringone.. stringtwo.. "!")
```

A way you could actually use this would be:

```other
print("This script's name is: ".. script.Name)
```

By the way, at any time you can use the variable “script” to refer to the current script the code is being executed in. That’s how script.Parent works.

---

**But now let's get into some more complicated stuff.**

String functions are more advanced ways to manipulate strings. Let’s look at a few. Starting with the basics, `string.lower()` changes the content of a string to lowercase. It's used like this:

```other
local mystring = "HELLo WorLD"
string.lower(mystring)
```

Like we learned in the functions lesson, just calling this by its self isn’t going to do anything. To actually use it, we could either set a variable to the result, or use it directly (without setting a variable)

```other
local string = "THIS IS A STRING THaT WiLL bE CoNVERTED to all LOWERCASE."
local newstr = string.lower(string) -- Set a variable to the lowercase string.
print(newstr) -- Print that variable
-- If you just wanted to replace the current varible then you can do
local string = "THIS IS A STRING THaT WiLL bE CoNVERTED to all LOWERCASE."
string = string.lower(string)
print(string)
```

Some more functions:

`string.upper(string)`  - Used in a similar way to string.lower

`string.len(string)`  - Returns the number of characters in a string.

`string.reverse(string)` - Returns a reversed version of the string.

`string.sub(string, startnum, endnum)` - Returns the substring found in between a start and end point. For example, `string.sub(“abcdefghijkl”, 4, 7)` would return “defg”

`string.gsub(string, find, replace)` - This function is much more than meets the eye, but at it's most basic level, it can find and replace something in a string. Here's an example:

```other
local string = "Hello world!"
local newstr, replaced = string.gsub(string, "Hello", "hi") -- This will create two variables because string.gsub returns two different things.
print("Replaced ".. replaced.. " substring(s).")
print("Result: ".. newstr)
--[[
This is a block comment by the way, anything in here will also be a comment.
Expected output:
>Replaced 1 substring(s)
>hi world!
]]
```

There’s a ton of other string functions, but that’s all we have time for today.

