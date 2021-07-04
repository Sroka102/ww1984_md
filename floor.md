### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Dance Floor

## Step 1
The colors on the wall seem to match the colors on the floor. Help Wonder Woman move over the colored blocks in the same sequence as seen on the wall. That should unlock a secret door on the back wall.

**Blocks Available:**  
``||ww:Move <direction> by <number>||`` - Wonder Woman will move in that *direction* the given *number* of blocks.  
``||ww:Turn <direction>||`` - Wonder Woman will turn in the given *direction*.  
``||loops:repeat <number> times||`` - Repeat code the given *number* of times.  

```ghost
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
    for (let index = 0; index < 4; index++) {
        
    }
})
```
```template
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(RIGHT_TURN)
})
```
```package
minecraft-ww1984=github:ReWrite-Media/ww1984-ts
```
