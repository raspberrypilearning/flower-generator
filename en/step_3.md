## Generate a flower

First you're going to generate a flower which can be drawn on the screen. 

--- task ---

Create a new Scratch project and delete the cat sprite.

[[[generic-scratch-new-project]]]

--- /task ---

--- task ---

Now you will use the Paint tool to create a new sprite shaped like a flower petal.

Click **Paint new sprite** and rename it as "Flower".

[[[generic-scratch-rename-sprite]]]

--- /task ---

--- task ---

In the Paint tool, switch to **Vector** mode by clicking **Convert to Vector**.

Use the Ellipse tool to draw a petal shape filled in orange (you'll use code to add more colour later). 

 ![screenshot](images/flower-petal.png)

 Note: Shapes created using Vector mode look neater when you change their size. 

--- /task ---

--- task ---

Add the following code to your Flower sprite to `stamp`{:class="blockpen"} a flower with six equally rotated petals when you `click the green flag`{:class="blockcontrol"}. 

![screenshot](images/flower-6-straight.png)

```blocks
when green flag clicked
repeat (6) 
  stamp
  turn cw (60) degrees
end
```

--- /task ---

You may find that your petals are offset in an odd way:

![screenshot](images/flower-6-offset.png)

This is because the sprite is being rotated around its centre. 

--- task ---

Change where the middle of your petal shape is using the crosshair tool:

![screenshot](images/flower-crosshair-annotated.png)

The crosshair should be at the bottom of the petal. 

--- /task ---

--- task ---

Before you run your code again, you should `clear`{:class="blockpen"} the stage so you can see your new flower.

Click on the `clear` block in the Pen tab.

```blocks
clear
```

--- /task ---

--- task ---

Run your code again to check that the petals are straight.

![screenshot](images/flower-6-straight.png)
 
--- /task ---
