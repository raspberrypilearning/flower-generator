## Challenge: custom flower blocks

These flowers all have the same number of outer and inner petals, and the size of the inner flower is in proportion to the outer flower: 
 
![screenshot](images/flower-double-flowers.png)

They were created using `draw double flower`{:class="blockmoreblocks"} custom block with inputs for `outer colour`, `inner colour`, and `size`.

```blocks
define draw double flower (outer colour) (inner colour) (size)
draw flower (outer colour) (size) (12) :: custom
draw flower (inner colour) ((size) / (2)) (20) :: custom
```

The `draw double flower`{:class="blockmoreblocks"} block was then used to draw lots of flowers in the same style:

```blocks
when [d v] key pressed
clear
go to x: (-100) y: (0)
draw double flower (160) (120) (100) :: custom
change x by (100)
draw double flower (120) (140) (75) :: custom
change x by (75)
draw double flower (140) (160) (50) :: custom
```

Can you create a new custom block for a kind of flower that you like, and add the inputs that you want to be able to change it? 

Then create a design that you like using your new block. 

