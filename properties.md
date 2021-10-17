So, you want to change properties of your Instance? This would let you change the name, color, collision rules, etc of any part or Instance. It’s actually pretty simple.

The easiest way is to insert a script inside of the thing that you want to the change the properties of. We'll be starting with a part, because it's easy to understand. Make sure you've created the part in the workspace. Once you have, hover over it in the explorer and click the plus button. Then search up script and select the option called "Script" not “LocalScript” or “ModuleScript".

Now delete the first line that says print(“Hello World”) and instead type script.parent.Transparency = 1.

When you run the game, this will make your part disappear. It’s still there, just invisible. That’s just one example of something you can do though. Let’s try some more!

```lua
-- Change the instance's name

script.Parent.Name = "NewName"

-- Change the part's Color

script.Parent.BrickColor = BrickColor.red() -- There's a lot more to this, and we'll cover this later

-- Change if the part can be collided with or not

script.Parent.CanCollide = false

-- Change if the part is anchored or not. Anchored parts won't fall or be affected by physics.

script.Parent.Anchored = true
```

> You can also use these properties on Variables, which means that the script won’t have to be inside of the part.

```lua
local part = game.Workspace.MyPart

part.Name = "TotallyEpicNewName"
```

Cool right? I promise that you’ll use this **all the time in your scripting.**

Next up is a short lesson on how to add [delays]() to your scripts!