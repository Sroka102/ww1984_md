### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Dance Floor

## Step 1
Kolory na ścianie wydają się pasować do kolorów na podłodze. Pomóż Wonder Woman przejść po kolorowych blokach w kolejności pokazanej na ścianie. To powinno otworzyć sekretne drzwi w tylnej ścianie.

**Dostępne Bloki:**  
``||ww:Idź <w kierunku> <ilość> kroków||`` - Wonder Woman poruszy sie *w kierunku* o *ilość* kroków. 
``||ww:Obróć <w kierunku>||`` - Wonder Woman obruci się w podanym *kierunku*.   
``||loops:powtórz <ile> razy||`` - Powtarza fragment kodu podaną *ilość* razy.   

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
minecraft-ww1984=github:Sroka102/ww1984-ts
```
