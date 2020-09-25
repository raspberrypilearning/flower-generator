## Zufälliger Blumengenerator

Du wirst nun deinen `Blume zeichnen`{:class="block3myblocks"}-Block benutzen, um hundert zufällige Blumen auf der gesamten Bühne zu erstellen, wann immer du <kbd>r</kbd> drückst.

![zufällige Blumen](images/flower-random.png)

\--- task \---

Füge deinem Code der Figur einen neuen Event-Block hinzu, so dass `Wenn Taste f gedrückt wird`{:class="block3events"}, der Bildschirm `geleert`{:class="block3extensions"} ist.

![Blumen-Figur](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

\--- /task \---

\--- task \---

Füge einen `Wiederhole 100 mal`{:class="block3control"}-Block ein, um zu einer `Zufallsposition zu gehen`{:class="block3motion"}.

![Blumen-Figur](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

\--- /task \---

\--- task \---

Verwende den `Blume zeichnen`{:class="block3myblocks"}-Block, um eine Blume zu erstellen, die eine `zufällige`{:class="block3operators"} Farbe zwischen `0` und `199` hat.

Dein Code sollte jetzt so aussehen:

![Blumen-Figur](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (100) (12) :: custom
end
```

\--- /task \---

Dieser Code erzeugt hundert Blumen mit unterschiedlichen Farben, aber mit der gleichen Größe und Anzahl von Blüten.

![Blumen mit zufälligen Farben](images/flower-random-colour.png)

\--- task \---

Kannst du das `Wenn Taste r gedrückt wird`{:class="block3events"}-Skript ändern, sodass die Größe und Anzahl der Blütenblätter ebenfalls zufällig sind?

\--- hints \---

\--- hint \---

Der `Blume zeichnen`{:class="block3myblocks"}-Block sollte `zufällig`{:class="block3operators"} die Anzahl und Größe der Blütenblätter wählen.

\--- /hint \---

\--- hint \---

Die folgenden Blöcke wählen eine zufällige Größe zwischen `50` und `150` und eine zufällige Anzahl an Blütenblättern zwischen `4` und `12`.

![Blumen-Figur](images/flower-sprite.png)

```blocks3
(Zufallszahl von (50) bis (150))

(Zufallszahl von (4) bis (12))
```

\--- /hint \---

\--- hint \---

Dein Code sollte so aussehen:

![Blumen-Figur](images/flower-sprite.png)

```blocks3
Wenn Taste  [r v] gedrückt wird
lösche alles
wiederhole (100) mal 
  gehe zu (Zufallsposition v)
  Blume zeichnen (Zufallszahl von (0) bis (199)) (Zufallszahl von (50) bis (150)) (Zufallszahl von (4) bis (12)) :: custom
end
```

\--- /hint \---

\---/hints\---

\--- /task \---

\--- task \---

Drücke <kbd>r</kbd>, um deine zufälligen Blume zu sehen.

\--- /task \---