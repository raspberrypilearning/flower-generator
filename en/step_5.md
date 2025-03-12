## Custom sizes and petals

--- task ---

Right-click on the `draw flower`{:class="block3myblocks"} definition block and choose **edit**. Add another input to set the size of the flower, so your `draw flower`{:class="block3myblocks"} block looks like this:

```blocks3
draw flower (180) (150) :: custom
```
--- /task ---

--- task ---

Change your `define draw flower`{:class="block3myblocks"} script to use the input you just added to set the flower's size:

```blocks3
define draw flower (colour) (size :: custom-arg)
set [color v] effect to (colour :: custom-arg)
+set size to (size :: custom-arg) %
repeat (6) 
  stamp
  turn cw (60) degrees
end
```
--- /task ---

--- task ---

In the `when green flag clicked`{:class="block3events"} script, change the second number in both `draw flower`{:class="block3myblocks"} blocks so that the two flowers appear in different sizes.

```blocks3 
when green flag clicked
erase all
go to x: (75) y: (75)
+draw flower (180) (150) :: custom
go to x: (-75) y: (-75)
+draw flower (150) (50) :: custom
```
--- /task ---

--- task ---

Test your code to check whether the flowers have different sizes.

--- /task ---

You can use an input to choose the number of petals a flower has.

--- task ---

Right-click on the `draw flower`{:class="block3myblocks"} definition block and choose **edit**. Add another input for the number of petals.

--- /task ---

--- task ---

Change the `draw flower`{:class="block3myblocks"} definition to create the number of petals specified by the new input.

```blocks3
define draw flower (colour) (size :: custom-arg) (petals)
set [color v] effect to (colour :: custom-arg)
set size to (size :: custom-arg) %
+repeat (petals :: custom-arg) 
  stamp
  +turn cw ((360) / (petals :: custom-arg)) degrees
end
```

--- /task ---

--- task ---

In the `when green flag clicked`{:class="block3events"} script, change the third number in both `draw flower`{:class="block3myblocks"} blocks so that the two flowers that appear have different numbers of petals.

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
+draw flower (180) (150) (3) :: custom
go to x: (-75) y: (-75)
+draw flower (150) (50) (8) :: custom
```

--- /task ---

--- task ---

Add more `draw flower`{:class="block3myblocks"} blocks to your program to draw flowers with different colours, sizes, and numbers of petals all over the Stage.

--- /task ---
