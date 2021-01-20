## Generador aleatorio de flores

Ahora usarás tu bloque `dibuja flor`{:class="block3myblocks"} para crear muchas flores de manera aleatoria por todo el Escenario cada vez que presionas <kbd>r</kbd>.

![flores aleatorias](images/flower-random.png)

--- task ---

Agrega un nuevo bloque de Evento al código de tu objeto para que `al presionar la tecla r`{:class="block3events"}, la pantalla se `borré`{:class="block3extensions"}.

![objeto flor](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

--- /task ---

--- task ---

Añadir el bloque `repetir`{:class="block3control"} para ir a una `posición aleatoria`{:class="block3motion"} `100` veces.

![objeto flor](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

--- /task ---

--- task ---

Usa el bloque `dibuja flor`{:class="block3myblocks"} para crear una flor que tenga un color `aleatorio`{:class="block3operators"} entre `0` y `199`.

Tu código ahora deberá verse así:

![objeto flor](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  dibuja flor (pick random (0) to (199)) (100) (12) :: custom
end
```

--- /task ---

Este código crea cien flores con diferentes colores pero con el mismo tamaño y número de pétalos.

![sólo flores con colores aleatorios](images/flower-random-colour.png)

--- task ---

¿Puedes modificar el texto `cuando se presiona la tecla r`{:class="block3events"}, para que el tamaño de las flores y el número de pétalos también sean aleatorios?

--- hints ---


--- hint ---

El bloque `dibuja flor`{:class="block3myblocks"} debe elegir un `número al azar entre`{:class="block3operators"} para el tamaño y el número de pétalos.

--- /hint ---

--- hint ---

Los siguientes bloques toman un tamaño aleatorio entre `50` y `150` y un número aleatorio de pétalos entre `4` y `12`.

![objeto flor](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

--- /hint ---

--- hint ---

Tu código debería verse así:

![objeto flor](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  dibuja flor (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

Presiona <kbd>r</kbd> para ver tus flores generadas de manera aleatoria.

--- /task ---