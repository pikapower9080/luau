Remember that one function we learned called print? Well, here I'm going to show you how to properly use functions and even how to make your own!

**Custom Functions**

First let's start with custom functions. These are blocks of code that you can run twice without having to type it twice, it's like a variable but for blocks of code! They can also have arguments. For example if you wanted to run the code one time but with one thing that made it different than the second time you ran it, you could!

To declare a function, type the following:

```lua
function myFunctionName(argument, anotherArgument, yetAnotherArgument)

end
```

The function tells the computer that it's a function, the myFunctionName can be changed to whatever you want (it's what you'll type to run your function and yes it follows the same naming rules and variables) and the stuff in the brackets are the arguments! These can be called whatever you want BUT YES THEY HAVE TO FOLLOW VARIABLE NAMING RULES GEE and you can use them like they were variables while you are writing your function.

Let's start by writing a function to print a custom message (yes I know you're tired of this but you have to learn some way). We will create a function called printMessage with the message argument that will print whatever message you tell it to.

```lua
function printMessage(message)
    print(message)
end
```

Now, this won't do anything on it's own. To make it run we can type the following:

```lua
printMessage("Yo!")
```

This will print the message "Yo!" to the output This is because it ran the code inside the function (which was to print message) and you used the first argument which the function saw as message to print whatever you wanted! Now the advantage of this is that you can run lots of code but with just one tweak and you don't have to write it again. Check this out:

```lua
function printMessage(message)
    print(message)
end

printMessage("Message1")
printMessage("Message2")
printMessage("Message3")
--[[
    Expected output:
    Message1
    Message2
    Message3
]]
```

But functions don't have to have arguments, they can just be easy ways to execute a bunch of code! Here's an example:

```lua
function longFunction()
    print("Do some stuff")
    print("Do some more stuff")
    print("do even more stuff")
    print("I'm starting to get bored")
end

longFunction() -- Now we've ran it once
longFunction() -- And twice! That just saved us four lines of code
```

So there you have it, custom functions!

**Built in functions**

Built in functions are functions like print() that are already set by the game engine some examples are:

Here are a couple of examples of built in functions:

-wait(Seconds)
-spawn(function)
-pcall(function)
-tostring(number)
-tonumber(string)
-Instance.new()

And that's just the tip of the iceberg, I could add more to the list but it doesn't really matter.

**Instance functions**

These are functions that are part of an instance (which just means an object like a part, script, model, anything). They are called with Instance:function(). A common one is instance:Destroy() it will remove the object completely. Another one is instance:Clone() which will create a copy of the instance (You will need to parent it into workspace or something else like I show in the example)

```lua
local clone = game.Workspace.MyPart:Clone()
clone.Parent = workspace
-- Oh yeah, did I mention you can just type workspace instead of game.Workspace? I still use the ladder though
```

**And finally, returning**

Returning is when a function will return a value after being called. For example, if you were to make a function to get the name of a part, it might look something like this

```lua
function getPartName(part)
    return part.Name
end

-- Now, to get the returned value you can use a variable like this:

local returnedPartName = getPartName(game.Workspace.MyPart)

print(returnedPartName)

-- Expected output: MyPart
```

So, that's all for now, There's more to cover but I'll save that for another time.

Our next lesson is about [instancing](/instancing.md), and important part of roblox coding. See you there!