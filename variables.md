# Roblox luau guide

Oh boy! Time to learn about something really cool in scripting! Variables! As you might know from math class, a variable is a value that is able to be changed. That's true, but in scripting it can also be used as a shortcut, I'll tell you what I mean in a bit.

But first, let's learn about how it can be used normally. This is the most simple example, and quite frankly it's kind of useless to make the variable but hey I don't make the rules.

For some reason there is such thing as a global variable that you can declare as

Variable = value

But for some reason nobody uses those and they can't be declared most of the time, just at the top of the script basically. Most people just use a local variable, which as long as it's not declared inside a function, it's good to go as a global one. For real, I've only ever seen people use local variables, even if there's no reason. Here's how you use a local variable.

```lua
local message = "Hello!"
print(message)
-- Expected output: Hello! 

-- Did I mention these things are comments?
-- If you put two dashes anywhere on a line, from that point foward the line is a comment. This means that computer will ignore it! More on that later.
```

The beauty of that is that if you change the message variable, manually or using an assignment (more on that later) then it will update the print message too! If you had multiple print messages, it would update for all of those that used the message variable as well!

```lua
local message = "Hey!"
print(message)
print(message)
print(message)
--[[
    Expected output:
    Hey!
    Hey!
    Hey!
]]
```

This is useful for if you have something that you're going to type over and over and you don't feel like typing it that many times. That's also what I meant when I said it could be used as a shortcut. Let's put this in action!

First: Make a new part in the workspace by clicking the part button in the home tab. Then rename it by right clicking it in the explorer and clicking rename. Make sure it does not share a name with any other part in the workspace. I'll call mine "MyPart". By the way, when scripting it's much easier to name your parts usingCamelCaseLikeThisWhereThereAreNoSpacesOrSpecialCharactersButEveryNewWorkIsAnotherCapitalLetterSoYouCanReadIt

**Variables also have to be named like this but they can contain numbers, as long as they don't start with them.**

<video controls>
    <source src="/assets/newpart.mp4" type="video/mp4"></source>
</video>

Now, let's do something with this part. We can print the name of it, and use a variable to locate it. Create a new script and type:

```lua
local part = game.Workspace.MyPart
print(part.Name)
```

(If you picked a different name than MyPart for your part name then change the game.Workspace.MyPart to your part's name)

Now if you run the game it should print "MyPart" to the output. Let's try something else now. Make another part and call it "OtherPart" or something else that isn't already in use. Now change the line that says local part = game.Workspace.MyPart to local part = game.Workspace.OtherPart then run the game and you should see it changed to other part! That's the magic of variables!

Next up we'll be learning about [functions](/functions.md), which are like variables for code. See you there!