### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true 
### @explicitHints 1

# Beams of Color

## Step 1
Pomóż Wonder Woman umieścić szklane bloki na wiązkach światła, aby dopasować kolor do wzoru widocznego na ścianie. Musisz jej powiedzieć, gdzie ma się poruszać i jakie kolory umieścić. 

**Dostępne Bloki:**  
``||ww:Idź <w kierunku> <number> kroków||`` - Wonder Woman poruszy sie w *kierunku* *ilosc* kroków.  
``||ww:Obróć <w kierunku>||`` - Wonder Woman obruci się w podanym *kierunku*.  
``||ww:Umieść <kolor szklanego bloku> <w kierunku>||`` - Umieszcza blok kolorowego szkła w ustalonym kierunku.  
``||loops:powtórz <ile> razy||`` - Powtarza ustalony fragment kodu podaną *ilość* razy.  

```ghost
player.onChat("run", function () {
    for (let index = 0; index < 4; index++) {
        ww.moveWW(Direction.Forward, 1)
        ww.turnWW(LEFT_TURN)
        ww.placeBlock(BeamsGlass.YellowStainedGlass, Direction.Forward)
    }
})
```
```template
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.LimeStainedGlass, Direction.Right)
})
```
```package
minecraft-ww1984=github:Sroka102/ww1984-ts
```