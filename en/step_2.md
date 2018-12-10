## Generate a flower

First you're going to generate a flower that can be drawn on the Stage. 

--- task ---

Create a new Scratch project, and delete the cat sprite.

[[[generic-scratch3-new-project]]]

--- /task ---

--- task ---

Add the **Pen** extension to your project.

[[[generic-scratch3-add-pen-extension]]]

--- /task ---

--- task ---

Now use the Paint tool to create a new sprite shaped like a flower petal.

Click on **Paint new sprite** and rename it 'Flower'.

[[[generic-scratch3-rename-sprite]]]

--- /task ---

--- task ---

Use the Circle tool to draw a petal shape filled in orange. 

![screenshot](images/flower-petal.png)

Later, you will use code to add more colour.

--- /task ---

--- task ---

Add the following code to the Flower sprite to `stamp`{:class="block3extensions"} a flower with six equally rotated petals `when the green flag is clicked`{:class="block3control"}. 

![screenshot](images/flower-6-straight.png)

```blocks3
when green flag clicked
repeat (6) 
  stamp
  turn cw (60) degrees
end
```

--- /task ---

You may find that your petals are arranged in an odd way:

![screenshot](images/flower-6-offset.png)

This is because the sprite is being rotated around its centre. 

--- task ---

Move your petal so the bottom is in the centre.

![screenshot](images/flower-crosshair-annotated.png)

You may find it easier to zoom out to do this.

--- /task ---

Before you run your code again, you should `clear`{:class="block3extensions"} the Stage.

--- task ---

Click on the `clear` block in the Pen tab.

```blocks3
clear
```

--- /task ---

--- task ---

Run your code again to check that the flower's petals are straight now.

![screenshot](images/flower-6-straight.png)

If not, adjust the petals position until it is in the centre.
 
--- /task ---
