## Desafío: bloques de flores personalizados

Todas estas flores tienen el mismo número de pétalos externos e interiores, y el tamaño de la flor interna es proporcional a la flor externa:

![captura de pantalla](images/flower-double-flowers.png)

Puedes crear flores como esta con la ayuda del bloque personalizado `dibuja una flor doble`{:class="block3myblocks"} que tiene entradas para `color exterior`, `color interno`, y `tamaño`:

```blocks3
define draw double flower (outer colour) (inner colour) (size :: custom-arg)
draw flower (outer colour :: custom-arg) (size :: custom-arg) (12) :: custom
draw flower (inner colour :: custom-arg) ((size :: custom-arg) / (2)) (20) :: custom
```

El bloque `dibuja una flor doble`{:class="block3myblocks"} puede dibujar un montón de flores del mismo estilo:

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

Crea un nuevo bloque personalizado con las entradas necesarias que necesites cambiar para crear el tipo de flor que quieras.

¡Después usa tu nuevo bloque para crear un diseño genial!