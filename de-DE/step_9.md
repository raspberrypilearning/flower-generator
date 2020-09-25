## Herausforderung: benutzerdefinierte Blumen-Blöcke

Diese Blumen haben alle die gleiche Anzahl an äußeren und inneren Blüten, und die Größe der inneren Blume ist proportional zur äußeren Blume:

![Bildschirmfoto](images/flower-double-flowers.png)

Du kannst Blumen wie diese mit Hilfe eines benutzerdefinierten Blocks `Doppelblume zeichnen`{:class="block3myblocks"} mit Eingaben für `Außenfarbe`, `Innenfarbe` und `Größe` erstellen:

```blocks3
define draw double flower (outer colour) (inner colour) (size :: custom-arg)
draw flower (outer colour :: custom-arg) (size :: custom-arg) (12) :: custom
draw flower (inner colour :: custom-arg) ((size :: custom-arg) / (2)) (20) :: custom
```

Der `Doppelte Blume zeichnen`{:class="block3myblocks"}-Block kann viele Blumen im gleichen Stil zeichnen:

```blocks3
when [d v] key pressed
erase all
go to x: (-100) y: (0)
draw double flower (160) (120) (100) :: custom
change x by (100)
draw double flower (120) (140) (75) :: custom
change x by (75)
draw double flower (140) (160) (50) :: custom
```

Erstelle einen neuen Block mit den notwendigen Eingaben, die du ändern musst, um eine Blume zu erstellen, die dir gefällt.

Benutze nun deinen neuen Block, um ein cooles Design zu erstellen!