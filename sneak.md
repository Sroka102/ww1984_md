### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Stealth Mission

## Step 1
Pomoz Wonder Woman przejsc przez pokoj bez wywolywania alarmu, unikaj laserow. Bedzie musiala sie zakrasc i obezwladnić przestepce.

**Dostępne Bloki:**  
``||ww:Idź <w kierunku> <ilość> kroków||`` - Wonder Woman poruszy sie *w kierunku* o *ilość* kroków. 
``||ww:Obróć <w kierunku>||`` - Wonder Woman obruci się w podanym *kierunku*.  
``||ww:Atakuj przestępcę <w kierunku>||`` - Bezszelestnie powali przestępcę atakując w podanym *kierunku*.  
``||loops:powtórz <ile> razy||`` - Powtarza fragment kodu podaną *ilość* razy.  

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
ww1984_md=github:Sroka102/ww1984_md
```
