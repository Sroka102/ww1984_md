### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Hidden in Plain Sight

## Step 1
Przestępca, który zaplanował napad, ukrywa się w tłumie. Pomóż Wonder Woman sprawdzić każdą osobę, aby dowiedzieć się, kto jest złodziejem w przebraniu. Następnie użyj lassa prawdy, aby uzyskać pojmać przestępcę i odzyskać ostatni element obrazu.

**Dostępne Bloki:**  
``||ww:Idź <w kierunku> <number> kroków||`` - Wonder Woman poruszy sie w *kierunku* *ilosc* kroków.  
``||ww:Obróć <w kierunku>||`` - Wonder Woman obruci się w podanym *kierunku*.   
``||ww:uczestnik jest złodziejem <w kierunku>||`` - Zwraca wartość boolowską (*prawda* | *fałsz*) zależnie od tego, czy uczestnik jest złodziejem czy nie.  
``||ww:Łap lassem złodzieja <w kierunku>||`` - Powoduje użycie przez Wonder Woman lassa prawdy na złodzieju w ustalonym *kierunku*.  
``||loops:powtórz <ile> razy||`` - Powtarza ustalony fragment kodu podaną *ilość* razy. 
``||loops:dopuki <wartość boolowska>||`` - Powtarza ustalony fragment kodu dopuki podana wartość boolowska ma wartość *prawda*.  
``||logic:jeśli / to||`` - Sprawdza czy warunek jest *prawda* , jeśli tak to wykonuje podane instrukcje.  
``||logic:nie <wartość boolowska>||`` - Zmienia wartość boolowską na przeciwną. Na przykład działanie warunku: *dopuki <prawda>* na *dopuki nie <prawda>*  

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
minecraft-ww1984=github:Sroka102/ww1984-ts
```
