## Generate a flower

First you're going to generate a flower that can be drawn on the Stage.

\--- uppgift \---

Create a new Scratch project, and delete the cat sprite.

[[[generic-scratch3-new-project]]]

\--- /task \---

\--- uppgift \---

Add the Pen extension to your project.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- uppgift \---

Now use the Paint tool to create a new sprite shaped like a flower petal.

Click on **Choose a sprite**, then click on **Paint** and rename the sprite 'Flower'.

[[[generic-scratch3-draw-sprite]]]

\--- /task \---

\--- uppgift \---

Use the Circle tool to draw a petal shape filled in orange.

![skärmdump](images/flower-petal.png)

Later, you will use code to add more colour.

\--- /task \---

\--- uppgift \---

Add the following code to the Flower sprite to `stamp`{:class="block3extensions"} a flower with six equally rotated petals `when the green flag is clicked`{:class="block3control"}.

![skärmdump](images/flower-6-straight.png)

```blocks3
when green flag clicked
repeat (6) 
  stamp
  turn cw (60) degrees
end
```

\--- /task \---

You may find that your petals are arranged in an odd way:

![skärmdump](images/flower-6-offset.png)

This is because the sprite is being rotated around its centre.

\--- uppgift \---

Move your petal so its bottom is in the centre.

![skärmdump](images/flower-crosshair-annotated.png)

Doing this may be easier if you zoom out.

\--- /task \---

Before you run your code again, you should `erase all`{:class="block3extensions"} the sprites on the Stage to clear it.

\--- uppgift \---

Click on the `erase all` block in the Pen blocks section.

```blocks3
erase all
```

\--- /task \---

\--- uppgift \---

Run your code again to check that the flower's petals are straight now.

![skärmdump](images/flower-6-straight.png)

If not, adjust the petal's position until its bottom in the centre.

\--- /task \---