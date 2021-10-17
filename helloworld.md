# Let's write our first script.

We're going to begin by creating a hello world script. This is a common practice when learning a new language. This will cause the words "Hello, world!" to be printed to the output. First, make sure the output is enabled by going into view and output. You don't have to have your layout like mine, it all comes down to how you like it.

![Image](/assets/enableoutput.gif)

Now that you have that out of the way, let's get making! First hover your mouse on the workspace in the explorer (If you don't see that do the same thing you did with the output but check explorer instead) Then click the plus and type script into the search box that pops up, then click on script and it should open in the window.

![Image](/assets/newscript.gif)

It should already have written your script for you! It may or my not have already had the words print("Hello, world!") packed in with it. But so that we can learn, Let's delete that line and write it again.

First, we're going to need to add a print function. A function is just something that tells something else to happen. You can make your own functions, but print is one of the built in ones. Now your script should look like this

```lua 
print()
```

But that's not going to do anything because it needs an argument. This argument tells the game what to print! You type the arguments inside of the brackets. Like this!

```lua
function(argument1, argument2)
```

Almost any time you're using a piece of text, be it in an argument or something else you're going to need to put it in quotes. This will make it a string! Strings can have most characters in them and can be combined with other strings like this:

```lua
print("Hello ".. "world!")
-- Expected output: Hello world!
```

Amazing right? Now, fill the print function with a string argument of "Hello, world!" Make sure you keep the quotes!

And now you're done! Run the game by pressing the guy at the top (You may need to close out of the script) and check the output!

