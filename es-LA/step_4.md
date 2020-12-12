## Personaliza tus flores

Hasta este momento, todas las flores que dibujas son exactamente iguales. A continuación añadirás algunas entradas al bloque `dibuja flor`{:class="block3myblocks"} para que puedas dibujar flores de diferentes colores, tamaños y números de pétalos.

\--- task \---

En Scratch puedes usar el bloque `fijar efecto color`{:class="block3looks"} para cambiar el color de un objeto.

Cambia tu definición de "dibujar una flor" para cambiar el color:

![objeto de flor](images/flower-sprite.png)

```blocks3
define draw flower
set [color v] effect to (150)
repeat (6) 
  stamp
  turn cw (60) degrees
end
```

\--- /task \---

\--- task \---

Ejecuta tu código para ver flores de diferentes colores.

![captura de pantalla](images/flower-pink.png)

`set colour effect`{:class="block3looks"} changes the colour based on the default colour of the sprite, so if your sprite doesn't start out orange, you get different results.

\--- /task \---

\--- task \---

Experimenta con el uso de diferentes números desde `0` a `199` en el bloque `fijar efecto color`{:class="block3looks"} y ve los diferentes resultados que obtienes.

\--- /task \---

Hasta el momento, todas las flores son del mismo color. Para darle a cada flor un color diferente, tienes que añadir un bloque **input** al bloque`dibuja flor`{:class="block3myblocks"}.

\--- task \---

Haz un clic derecho en el bloque de definición `dibuja flor`{:class="block3myblocks"} y selecciona **editar**:

![captura de pantalla](images/flower-edit.png)

\--- /task \---

\--- task \---

Ahora añade un **número de entrada** que se llame 'color':

![captura de pantalla](images/flower-colour-input-annotated.png)

La entrada aparece en la definición `dibuja flor`{:class="block3myblocks"}, y puedes arrastrarla a donde quieras usarla.

\--- /task \---

\--- task \---

Arrastra la entrada 'color' al bloque `fijar efecto color`{:class="block3looks"}:

![captura de pantalla](images/flower-use-colour-annotated.png)

Tu código debería verse así:

![objeto flor](images/flower-sprite.png)

```blocks3
define draw flower (colour)
set [color v] effect to (colour :: custom-arg)
repeat (6)
  stamp
  turn cw (60) degrees
end
```

\--- /task \---

Ten en cuenta que los bloques `dibuja flor`{:class="block3myblocks"} ahora tienen una nueva entrada establecida en `1`:

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
draw flower (1) :: custom
go to x: (-75) y: (-75)
draw flower (1) :: custom
```

\--- task \---

Cambia los números en los bloques `dibuja flor`{:class="block3myblocks"} para que las dos flores aparezcan en diferentes colores. Puedes elegir cualquier número entre 0 y 200.

Tu código debe parecerse a esto:

![objeto flor](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
draw flower (180) :: custom
go to x: (-75) y: (-75)
draw flower (150) :: custom
```

\--- /task \---

\--- task \---

Ahora añade otra entrada para establecer el tamaño de la flor, así que tu bloque `dibuja flor`{:class="block3myblocks"} se ve así:

![objeto flor](images/flower-sprite.png)

```blocks3
draw flower (180) (150) :: custom
```

Con el bloque de arriba, puedes crear flores con diferentes tamaños:

![flores de diferentes tamaños](images/flower-different-sizes.png)

\--- hints \---

\--- hint \---

Mira lo que hiciste para añadir la entrada `color`, y repítelo para añadir una entrada de 'tamaño' que puedes usar para establecer el tamaño del objeto flor.

\--- /hint \---

\--- hint \---

Editar el bloque `dibuja flor`{:class="block3myblocks"} para añadir una nueva entrada de número llamada 'tamaño'.

Necesitas añadir el siguiente bloque con una entrada de 'tamaño' al `dibuja flor`{:class="block3myblocks"} bloque de definición:

```blocks3
set size to (100) %
```

\--- /hint \---

\--- hint \---

Dale un clic derecho en el bloque de definición `dibuja flor`{:class="block3myblocks"}, haga clic en **editar**, y agrega un número de entrada llamado 'tamaño'.

![objeto flor](images/flower-sprite.png)

Cambia tu texto `definir dibuja flor`{:class="block3myblocks"} para que se vea así:

```blocks3
define draw flower (colour) (size :: custom-arg)
set [color v] effect to (colour :: custom-arg)
set size to (size :: custom-arg) %
repeat (6) 
  stamp
  turn cw (60) degrees
end
```

\--- /hint \---

\--- /hints \---

\--- /task \--- \--- task \---

En el bloque `al presionar ⚑`{:class="block3events"}, cambia el segundo número en ambos bloques `dibuja flor`{:class="block3myblocks"} para que así las dos flores aparezcan en diferentes tamaños.

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
draw flower (180) (150) :: custom
go to x: (-75) y: (-75)
draw flower (150) (50) :: custom
```

\--- /task \---

\--- task \---

Prueba tu código para comprobar si las flores tienen diferentes tamaños.

\--- /task \---

\--- task \---

Sería genial elegir el número de pétalos que tienen las flores.

Agrega otra entrada para que así puedas dibujar flores como esta:

![flores con diferentes números de pétalos](images/flower-petals.png)

\--- hints \--- \--- hint \---

Necesitas añadir una entrada de número de 'pétalos' y luego usarla en el bloque `definir dibuja flor`{:class="block3myblocks"}.

Hay dos lugares donde necesitas agregar la entrada de 'pétalos'.

El número de grados por los que el objeto Flores debe `girar`{:class="block3looks"} es `360` dividido entre el número de pétalos.

\--- /hint \---

\--- hint \---

Cambia tu bloque `definir dibuja flor`{:class="block3myblocks"} para que se vea así:

![objeto flor](images/flower-sprite.png)

```blocks3
define draw flower (colour) (size :: custom-arg) (petals)
```

Actualiza tus bloques `repetir`{:class="block3control"} y `girar`{:class="block3looks"} para que usen la entrada 'pétalos'.

```blocks3
repeat (petals :: custom-arg) 
end

turn cw ((360) / (petals :: custom-arg)) degrees
```

Actualiza tus bloques `dibuja flor`{:class="block3myblocks"} para usar la entrada 'pétalos'.

```blocks3
draw flower (150) (50) (8) :: custom
```

\--- /hint \---

\--- hint \---

Edita tu bloque `definir dibuja flor`{:class="block3myblocks"} y agrega una nueva entrada de número llamada 'pétalos'.

![objeto flor](images/flower-sprite.png)

Tu código debería verse así:

```blocks3
define draw flower (colour) (size :: custom-arg) (petals)
set [color v] effect to (colour :: custom-arg)
set size to (size :: custom-arg) %
repeat (petals :: custom-arg) 
  stamp
  turn cw ((360) / (petals :: custom-arg)) degrees
end

```

En el bloque `al presionar ⚑`{:class="block3events"}, cambia el tercer número en ambos bloques `dibuja flor`{:class="block3myblocks"} para que así las dos flores aparezcan tengan diferentes números de pétalos.

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
draw flower (180) (150) (3) :: custom
go to x: (-75) y: (-75)
draw flower (150) (50) (8) :: custom
```

\--- /hint \---

\--- /hints \---

\--- /task \---

A continuación, edita tu código para que puedas dibujar diferentes flores pulsando la tecla <kbd>f</kbd>.

\--- task \---

Ahora mueve tu código para dibujar flores desde abajo del bloque `al presionar ⚑`{:class="block3events"}, y poner el código bajo el bloque `al presionar la tecla f`{:class="block3events"}.

![objeto flor](images/flower-sprite.png)

```blocks3
when green flag clicked
```

```blocks3
when [f v] key pressed
erase all
go to x: (75) y: (75)
draw flower (180) (150) (3) :: custom
go to x: (-75) y: (-75)
draw flower (150) (50) (8) :: custom
```

\--- /task \---

\--- task \---

Pulsa <kbd>f</kbd> para probar tu código.

\--- /task \---

\--- task \---

Añade más bloques `dibuja flor`{:class="block3myblocks"} a tu programa para dibujar flores con diferentes colores, tamaños y números de pétalos por todo el Escenario.

\--- /task \---