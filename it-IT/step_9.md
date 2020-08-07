## Sfida: blocchi personalizzati per creare fiori

Questi fiori hanno tutti lo stesso numero di petali esterni e interni, e la dimensione del fiore interno è proporzionale al fiore esterno:

![schermata](images/flower-double-flowers.png)

Puoi creare fiori come questo con l'aiuto di un blocco personalizzato `disegna un fiore doppio`{:class="block3myblocks"} che ha argomenti per `colore esterno`, `colore interno`, e `dimensione`:

```blocks3
define disegna un fiore doppio (colore esterno) (colore interno) (dimensione :: custom-arg)
disegna un fiore (colore esterno :: custom-arg) (dimensione :: custom-arg) (12) :: custom
disegna un fiore (colore interno :: custom-arg) ((dimensione :: custom-arg) / (2)) (20) :: custom
```

Il blocco `disegna un fiore doppio`{:class="block3myblocks"} può disegnare molti fiori nello stesso stile:

```blocks3
when [d v] key pressed
erase all
go to x: (-100) y: (0)
disegna un fiore doppio (160) (120) (100) :: custom
change x by (100)
disegna un fiore doppio (120) (140) (75) :: custom
change x by (75)
disegna un fiore doppio (140) (160) (50) :: custom
```

Crea un nuovo blocco personalizzato con gli argomenti necessari a creare un tipo di fiore che ti piace.

Adesso usa il tuo nuovo blocco per creare un bel disegno!