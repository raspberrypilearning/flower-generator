## Crea un bloque personalizado para dibujar flores

¿Qué pasa si quieres dibujar muchas flores? En lugar de hacer muchas copias del código, crearás tu propio bloque en Scratch y lo usarás cada vez que quieras dibujar una flor.

--- task ---

Haz clic en **Mis Bloques** y luego en **Crea un Bloque** para crear tu propio bloque llamado 'dibuja flor'.

![captura de pantalla](images/flower-make-block.png)

--- /task ---

--- task ---

Ahora hay un nuevo bloque llamado `dibuja flor`{:class="block3myblocks"} en la sección **Más bloques** y un nuevo bloque de definición en el escenario.

```blocks3
dibuja flor :: custom

define dibuja flor
```

--- /task ---

--- task ---

Mueve tu código para dibujar la flor desde el bloque `al presionar ⚑`{:class="block3events"} al nuevo bloque `dibuja flor`{:class="block3myblocks"} bloque de definición.

Tu código debería verse así:

![objeto flor](images/flower-sprite.png)

```blocks3
define dibuja flor
repeat (6) 
  stamp
  turn cw (60) degrees
end

when green flag clicked
```

--- /task ---

--- task ---

Añade el siguiente código para limpiar el Escenario y usar tu nuevo bloque `dibuja flor`{:class="block3myblocks"} cuando se haga clic en la bandera verde:

![objeto flor](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
dibuja flor :: custom
```

--- /task ---

--- task ---

Dale clic a la bandera verde para poner a prueba tu código y verificar si es que ves una flor.

--- /task ---

--- task ---

Ahora cambia tu código para mover el objeto y luego dibuja otra flor:

![objeto flor](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
dibuja flor :: custom
go to x: (-75) y: (-75)
dibuja flor :: custom 
```

--- /task ---

--- task ---

Prueba tu código para comprobar que ahora ves dos flores.

![captura de pantalla](images/flower-two.png)

--- /task ---