## Willekeurige bloemgenerator

Je gebruikt nu je `teken bloem`{:class="block3myblocks"} blok om honderd willekeurige bloemen over het hele speelveld te maken wanneer je op de <kbd>r</kbd> drukt.

![willekeurige bloemen](images/flower-random.png)

\--- task \---

Voeg een nieuw gebeurtenisblok toe aan de code van je sprite zodat `wanneer r is ingedrukt`{:class="block3events"}, het scherm `gewist`{:class="block3extensions"} wordt.

![bloem sprite](images/flower-sprite.png)

```blocks3
wanneer [r v] is ingedrukt
wis alles
```

\--- /task \---

\--- task \---

Voeg een `herhaal`{:class="block3control"} blok toe om`100` keer naar een `willekeurige positie`{:class="block3motion"} te gaan.

![bloem sprite](images/flower-sprite.png)

```blocks3
herhaal (100)
  ga naar (willekeurige positie v)
einde
```

\--- /task \---

\--- task \---

Gebruik het blok `teken bloem`{:class="block3myblocks"} om een bloem te maken met een `willekeurige`{:class="block3operators"} kleur tussen `0` en `199`.

Je code zou er nu als volgt uit moeten zien:

![bloem sprite](images/flower-sprite.png)

```blocks3
wanneer [r v] is ingedrukt
wis alles
herhaal (100) 
  ga naar (willekeurige positie v)
  teken bloem (willekeurig getal tussen (0) en (199)) (100) (12) :: custom
einde
```

\--- /task \---

Deze code maakt honderd bloemen met verschillende kleuren maar met dezelfde grootte en hetzelfde aantal bloemblaadjes.

![bloemen met willekeurige kleuren](images/flower-random-colour.png)

\--- task \---

Kun je het `wanneer r is ingedrukt`{:class="block3events"} script wijzigen zodat de grootte en het aantal blaadjes van de bloemen ook willekeurig zijn?

\--- hints \---

\--- hint \---

Het `teken bloem`{:class="block3myblocks"} blok moet `willekeurige`{:class="block3operators"} nummers kiezen voor de grootte en het aantal blaadjes.

\--- /hint \---

\--- hint \---

De volgende blokken kiezen een willekeurige grootte tussen `50` en `150` en een willekeurig aantal blaadjes tussen `4` en `12`.

![bloem sprite](images/flower-sprite.png)

```blocks3
(willekeurig getal tussen (50) en (150))

(willekeurig getal tussen (4) en (12))
```

\--- /hint \---

\--- hint \---

Je code zou er als volgt uit moeten zien:

![bloem sprite](images/flower-sprite.png)

```blocks3
wanneer [r v] is ingedrukt
wis alles
herhaal (100) 
  ga naar (willekeurige positie v)
  teken bloem (willekeurig getal tussen (0) en (199)) (willekeurig getal tussen (50) en (150)) (willekeurig getal tussen (4) en (12)) :: custom
einde
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Druk op <kbd>r</kbd> om willekeurige bloemen te zien.

\--- /task \---