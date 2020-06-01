## Personaliza tus flores

Hasta este momento, todas las flores que dibujas son exactamente iguales. A continuación añadirás algunas entradas al bloque `dibujar flor`{:class="block3myblocks"} para que puedas dibujar flores de diferentes colores, tamaños y números de pétalos.

\--- task \---

En Scratch puedes usar el bloque `fijar efecto de color`{:class="block3looks"} para cambiar el color de un objeto.

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

`establecer el efecto de color`{:class="block3looks"} cambia el color según el color predeterminado del objeto. Así que si tu objeto no empieza color naranja, obtendrás resultados diferentes.

\--- /task \---

\--- task \---

Experimenta con el uso de diferentes números desde `0` a `199` en el bloque `establecer efecto de color`{:class="block3looks"} y ve los diferentes resultados que obtienes.

\--- /task \---

At the moment all flowers are the same colour. Para darle a cada flor un color diferente, tienes que añadir un bloque **input** al bloque`dibuja la flor`{:class="block3myblocks"}.

\--- task \---

Haz un clic derecho en el bloque de definición `dibujar flor`{:class="block3myblocks"} y selecciona **editar**:

![captura de pantalla](images/flower-edit.png)

\--- /task \---

\--- task \---

Ahora añade un **número de entrada** que se llame 'color':

![captura de pantalla](images/flower-colour-input-annotated.png)

La entrada aparece en la definición `dibujar flor`{:class="block3myblocks"}, y puedes arrastrarla a donde quieras usarla.

\--- /task \---

\--- task \---

Arrastra la entrada 'color' al bloque `establecer efecto de color`{:class="block3looks"}:

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

Notice that your `draw flower`{:class="block3myblocks"} blocks now have a new input that is set to `1`:

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
draw flower (1) :: custom
go to x: (-75) y: (-75)
draw flower (1) :: custom
```

\--- task \---

Cambia los números en los bloques `dibujar flor`{:class="block3myblocks"} para que las dos flores aparezcan en diferentes colores. Puedes elegir cualquier número entre 0 y 200.

Your code should look similar to this:

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

Now add another input to set the size of the flower, so your `draw flower`{:class="block3myblocks"} block looks like this:

![flower sprite](images/flower-sprite.png)

```blocks3
draw flower (180) (150) :: custom
```

With the block above, you can create flowers with different sizes:

![different sized flowers](images/flower-different-sizes.png)

\--- hints \---

\--- hint \---

Look at what you did to add the `colour` input, and repeat it to add a 'size' input that you can use to set the size of the Flower sprite.

\--- /hint \---

\--- hint \---

Edit the `draw flower`{:class="block3myblocks"} block to add a new number input called 'size'.

You need to add the following block with a 'size' input to the `draw flower`{:class="block3myblocks"} definition block:

```blocks3
set size to (100) %
```

\--- /hint \---

\--- hint \---

Right-click on the `draw flower`{:class="block3myblocks"} definition block, click on **edit**, and add a number input called 'size'.

![flower sprite](images/flower-sprite.png)

Change your `define draw flower`{:class="block3myblocks"} script so it looks like this:

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

In the `when green flag clicked`{:class="block3events"} script, change the second number in both `draw flower`{:class="block3myblocks"} blocks so that the two flowers appear in different sizes.

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

Test your code to check whether the flowers have different sizes.

\--- /task \---

\--- task \---

It would be cool to choose the number of petals the flowers have.

Add another input so that you can draw flowers like this:

![flowers with different numbers of petals](images/flower-petals.png)

\--- hints \--- \--- hint \---

You need to add a 'petals' number input, and then use it in the `define draw flower`{:class="block3myblocks"} block.

There are two places where you need to add the 'petals' input.

The number of degrees the Flower sprite should `turn`{:class="block3looks"} by is `360` divided by the number of petals.

\--- /hint \---

\--- hint \---

Change your `define draw flower`{:class="block3myblocks"} block to look like this:

![flower sprite](images/flower-sprite.png)

```blocks3
define draw flower (colour) (size :: custom-arg) (petals)
```

Update your `repeat`{:class="block3control"} and `turn`{:class="block3looks"} blocks so they use the 'petals' input.

```blocks3
repeat (petals :: custom-arg) 
end

turn cw ((360) / (petals :: custom-arg)) degrees
```

Update your `draw flower`{:class="block3myblocks"} blocks to use the 'petals' input.

```blocks3
draw flower (150) (50) (8) :: custom
```

\--- /hint \---

\--- hint \---

Edit your `define draw flower`{:class="block3myblocks"} block and add a new number input called 'petals'.

![flower sprite](images/flower-sprite.png)

Your code should look like this:

```blocks3
define draw flower (colour) (size :: custom-arg) (petals)
set [color v] effect to (colour :: custom-arg)
set size to (size :: custom-arg) %
repeat (petals :: custom-arg) 
  stamp
  turn cw ((360) / (petals :: custom-arg)) degrees
end

```

In the `when green flag clicked`{:class="block3events"} script, change the third number in both `draw flower`{:class="block3myblocks"} blocks so that the two flowers that appear have different numbers of petals.

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

Next, edit your code so you can draw different flowers by pressing the <kbd>f</kbd> key.

\--- task \---

Now move your code for drawing flowers away from below the `when green flag clicked`{:class="block3events"} block, and put the code under a `when f key pressed`{:class="block3events"} block.

![flower sprite](images/flower-sprite.png)

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

Press <kbd>f</kbd> to test your code.

\--- /task \---

\--- task \---

Add more `draw flower`{:class="block3myblocks"} blocks to your program to draw flowers with different colours, sizes, and numbers of petals all over the Stage.

\--- /task \---