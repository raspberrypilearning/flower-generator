## Maak een aangepast blok om bloemen te tekenen

Wat als je veel bloemen wilt tekenen? In plaats van veel kopieën van de code te maken, maak je je eigen blok in Scratch en gebruik je dit elke keer dat je een bloem wilt tekenen.

--- task ---

Klik op **Mijn blokken** en vervolgens op **Maak een blok** om je eigen blok te maken met de naam 'teken bloem'.

![schermafbeelding](images/flower-make-block.png)

--- /task ---

--- task ---

Er is nu een nieuw blok met de naam `teken bloem`{:class="block3myblocks"} in de sectie **Mijn blokken** en een nieuw definitieblok in het spelveld.

```blocks3
teken bloem :: custom

define teken bloem
```

--- /task ---

--- task ---

Verplaats je code voor het tekenen van de bloem van het `wanneer op de groene vlag wordt geklikt`{:class="block3events"} blok naar het nieuwe `teken bloem`{:class="block3myblocks"} definitieblok.

Je code zou er als volgt uit moeten zien:

![bloem sprite](images/flower-sprite.png)

```blocks3
define teken bloem
repeat (6) 
  stamp
  turn cw (60) degrees
end

when green flag clicked
```

--- /task ---

--- task ---

Voeg de volgende code toe om het speelveld te wissen en je nieuwe `teken bloem`{:class="block3myblocks"} blok te gebruiken wanneer op de groene vlag wordt geklikt:

![bloem sprite](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
teken bloem :: custom
```

--- /task ---

--- task ---

Klik op de groene vlag om je code te testen en controleer of je een bloem ziet.

--- /task ---

--- task ---

Wijzig nu je code om de sprite te verplaatsen en vervolgens een andere bloem te tekenen:

![bloem sprite](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
teken bloem :: custom
go to x: (-75) y: (-75)
teken bloem :: custom 
```

--- /task ---

--- task ---

Test je code om te controleren of je nu twee bloemen ziet.

![schermafbeelding](images/flower-two.png)

--- /task ---