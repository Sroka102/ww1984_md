### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Hidden in Plain Sight

## Step 1
The criminal who planned the heist is hidden among the crowd. Help Wonder Woman check each person to figure out which is the thief in disguise and then use the lasso of truth to get the final painting piece.

**Blocks Available:**  
``||ww:Move <direction> by <number>||`` - Wonder Woman will move in that *direction* the given *number* of blocks.  
``||ww:Turn <direction>||`` - Wonder Woman will turn in the given *direction*.  
``||ww:attendee is the thief <direction>||`` - Return a boolean (*true* | *false*) of whether the attendee is the thief or not.  
``||ww:Lasso thief <direction>||`` - Causes Wonder Woman to use her lasso of truth on the thief.  
``||loops:repeat <number> times||`` - Repeat code the given *number* of times.  
``||loops:while <boolean>||`` - Repeatedly run the code while the boolean is *true*.  
``||logic:if / then||`` - Checks if a condition is *true* and then does something if it is.  
``||logic:not <boolean>||`` - Switches the operation of a condition. Example: *while <true>* vs. *while not <true>*  

```ghost
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
    for (let index = 0; index < 4; index++) {
        
    }
    if (ww.locateGoon(Direction.Forward)) {
        ww.apprehendGoon(Direction.Forward)
    }
    while (!(false)) {
        
    }	
})
```
```template
player.onChat("run", function () {
    if (ww.locateGoon(Direction.Forward)) {

    }
})
```
```package
minecraft-ww1984=github:ReWrite-Media/ww1984-ts
```
