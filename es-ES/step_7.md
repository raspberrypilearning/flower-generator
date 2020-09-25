## Generador de flores aleatorio

Ahora usarás tu bloque `dibuja una flor`{:class="block3myblocks"} para crear un centenar de flores aleatorias por todo el Escenario cuando presiones la <kbd>r</kbd>.

![flores aleatorias](images/flower-random.png)

\--- task \---

Añade un nuevo bloque de eventos al código de tu objeto para que `cuando se presione la tecla r `{:class="block3events"}, la pantalla se `borre`{:class="block3extensions"}.

![objeto de flores](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

\--- /task \---

\--- task \---

Añadir en un bloque `repetir`{:class="block3control"} ir a una `posición aleatoria`{:class="block3motion"} `100` veces.

![objeto de flores](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

\--- /task \---

\--- task \---

Usa el bloque `dibuja la flor`{:class="block3myblocks"} para crear una flor que tenga un color `aleatorio`{:class="block3operators"} entre `0` y `199`.

Tu código debería parecerse a esto:

![objeto de flores](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (100) (12) :: custom
end
```

\--- /task \---

Este código crea cien flores con diferentes colores pero con el mismo tamaño y número de pétalos.

![flores sólo con colores aleatorios](images/flower-random-colour.png)

\--- task \---

¿Puedes modificar el script `cuando se presiona la tecla r `{:class="block3events"}, para que el tamaño de las flores y el número de petalos sean también aleatorios?

\--- hints \---

\--- hint \---

El bloque `dibuja una flor`{:class="block3myblocks"} debe `seleccionar aleatoriamente`{:class="block3operators"} numeros para el tamaño y el número de pétalos.

\--- /hint \---

\--- hint \---

Los siguientes bloques seleccionan un tamaño aleatorio entre `50` y `150` y un número aleatorio de petalos entre `4` y `12`.

![objeto de flores](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

\--- /hint \---

\--- hint \---

Tu código debe parecerse a esto:

![objeto de flores](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Pulsa <kbd>r</kbd> para ver tus flores al azar.

\--- /task \---