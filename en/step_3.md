## Make a custom block 

You can create your _own_ block in Scratch and use it every time you want to draw a flower.  

--- task ---

Click on **My Blocks** and then on **Make a Block** to create your own block called 'draw flower'.

![Scratch menu with an arrow to 'Make a Block' and a box around the 'My blocks' red menu option.](images/flower-make-block.png)

--- /task ---

--- task ---

There is now a new block called `draw flower`{:class="block3myblocks"} in the **More blocks** section, and a new definition block on the Stage.

```blocks3
draw flower :: custom

define draw flower
```

--- /task ---

--- task ---

Move your code for drawing the flower from the `when green flag clicked`{:class="block3events"} block to the new `draw flower`{:class="block3myblocks"} definition block. 

Your code should look like this:

![flower sprite](images/flower-sprite.png)

```blocks3
define draw flower
repeat (6) 
  stamp
  turn cw (60) degrees
end

when green flag clicked
``` 

--- /task ---

--- task ---

Add the following code to clear the Stage and to use your new `draw flower`{:class="block3myblocks"} block when the green flag is clicked:

![flower sprite](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
draw flower :: custom
```
 
--- /task ---

--- task ---

Click the green flag to test your code and check whether you still see a flower. 

--- /task ---

--- task ---

Now change your code to move the sprite and then draw another flower:

![flower sprite](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
+go to x: (75) y: (75)
draw flower :: custom
+go to x: (-75) y: (-75)
+draw flower :: custom 
```

--- /task ---

--- task ---

Click the green flag and check that you now see two flowers.

![Two orange flowers on a white background](images/flower-two.png)  
 
--- /task ---
