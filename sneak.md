### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Stealth Mission

## Step 1
Pomóż Wonder Woman przejść przez pokój bez wywoływania alarmu, unikaj laserów. Będzie musiała się zakraść i obezwładnić przestępcę.

**Blocks Available:**  
``||ww:Move <direction> by <number>||`` - Wonder Woman poruszy się w *kierunku* o *ilość* bloków.  
``||ww:Turn <direction>||`` - Wonder Woman will turn in the given *direction*.  
``||ww:Takedown criminal <direction>||`` - Stealthily knock out the criminal in the given *direction*.  
``||loops:repeat <number> times||`` - Repeat code the given *number* of times.  

```ghost
player.onChat("run", function () {
    for (let index = 0; index < 4; index++) {
        ww.moveWW(Direction.Forward, 1)
        ww.turnWW(LEFT_TURN)
        ww.takedownGoon(Direction.Forward)
    }
})
```
```template
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
})
```
```package
minecraft-ww1984=github:ReWrite-Media/ww1984-ts
```
