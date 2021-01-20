## Desafío: bloques de flores personalizados

Todas estas flores tienen el mismo número de pétalos externos e interiores, y el tamaño de la flor interna es proporcional a la de la flor externa:

![captura de pantalla](images/flower-double-flowers.png)

Puedes crear flores como esta con la ayuda de un bloque personalizado `dibuja flor doble`{:class="block3myblocks"} que tiene entradas para `color externo`, `color interno`, y `tamaño`:

```blocks3
define dibuja flor doble (color externo) (color interno) (tamaño :: custom-arg)
dibuja flor (color externo :: custom-arg) (tamaño :: custom-arg) (12) :: custom
dibuja flor (color interno :: custom-arg) ((tamaño :: custom-arg) / (2)) (20) :: custom
```

El bloque `dibuja flor doble`{:class="block3myblocks"} puede crear un montón de flores del mismo estilo:

```blocks3
when [d v] key pressed
erase all
go to x: (-100) y: (0)
dibuja flor doble (160) (120) (100) :: custom
change x by (100)
dibuja flor doble (120) (140) (75) :: custom
change x by (75)
dibuja flor doble (140) (160) (50) :: custom
```

Crea un nuevo bloque personalizado con las entradas necesarias que puedas cambiar para crear un tipo de flor que te guste.

¡Después usa tu nuevo bloque para crear un diseño genial!