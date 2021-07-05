### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true 
### @explicitHints 1

# Suspicious Crates

## Step 1
Pomóż Wonder Woman przejść przy skrzyniach i znaleźć brakujący fragment obrazu. Musi ona przesukać każdą skrzynię, jeśli odkryje tą z elementem obrazu, niech ją rozbije aby aby go odzyskać.

**Dostępne Bloki:**  
``||ww:Idź <w kierunku> <number> kroków||`` - Wonder Woman poruszy sie w *kierunku* *ilosc* kroków.  
``||ww:Obróć <w kierunku>||`` - Wonder Woman obruci się w podanym *kierunku*.  
``||ww:obraz w skrzyni <w kierunku>||`` - Sprawdza w ustalonym *kierunku* i zwraca wartość boolowską (*prawda* | *fałsz*) zależnie od tego, czy wykryje element obrazu wewnątrz skrzyni.  
``||ww:Rozbij skrzynię <w kierunku>||`` - Kieruje Wonder Woman aby odzyskała ukryty element obrazu z ustalonego *kierunku*.  
``||loops:powtórz <ile> razy||`` - Powtarza ustalony fragment kodu podaną *ilość* razy. 
``||loops:dopuki <wartość boolowska>||`` - Powtarza ustalony fragment kodu dopuki podana wartość boolowska ma wartość *prawda*.  
``||logic:jeśli / to||`` - Sprawdza czy warunek jest *prawda* , jeśli tak to wykonuje podane instrukcje.  
``||logic:nie <wartość boolowska>||`` - Zmienia wartość boolowską na przeciwną. Na przykład działanie warunku: *dopuki <prawda>* na *dopuki nie <prawda>*  

```ghost
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
    if (ww.locatePainting(Direction.Forward)) {
        ww.retrievePainting(Direction.Forward)
    }
    for (let index = 0; index < 4; index++) {
        
    }
    while (!(false)) {
        
    }	
})
```
```template
player.onChat("run", function () {
    if (ww.locatePainting(Direction.Forward)) {

    }
})
```
```package
minecraft-ww1984=github:Sroka102/ww1984-ts
```