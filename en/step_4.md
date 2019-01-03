
## Customise your flowers

At the moment all the flowers you draw are exactly the same. Next you're going to add some inputs to the `draw flower`{:class="block3myblocks"} block so that you can draw flowers with different colours, sizes, and numbers of petals. 

--- task ---

In Scratch you can use the `set colour effect`{:class="block3looks"} block to change the colour of a sprite. 

Change your 'draw flower' definition to change the colour: 

![flower sprite](images/flower-sprite.png)

![blocks_1545308798_2038562](images/blocks_1545308798_2038562.png)

--- /task ---

--- task ---

Run your code to see flowers of different colours.

 ![screenshot](images/flower-pink.png)  

 `set colour effect`{:class="block3looks"} changes the colour based on the default colour of the sprite, so if your sprite doesn't start out orange, you get different results. 
 
--- /task ---

--- task ---

Experiment with using different numbers from `0` to `199` in the `set colour effect`{:class="block3looks"} block, and see what different results you get.

--- /task ---

At the moment all flowers are the same colour. To give each flower a different colour, you need to add an **input** to the `draw flower`{:class="block3myblocks"} block. 

--- task ---

Right-click on the `draw flower`{:class="block3myblocks"} definition block and choose **edit**:
 
![screenshot](images/flower-edit.png)  
 
--- /task ---

--- task ---

Now add a **input number** called 'colour': 

![screenshot](images/flower-colour-input-annotated.png)  
 
The input appears in the `draw flower`{:class="block3myblocks"} definition, and you can drag it to where you want to use it.

--- /task ---

--- task ---

Drag the 'colour' input to the `set colour effect`{:class="block3looks"} block: 
 
![screenshot](images/flower-use-colour-annotated.png)

Your code should look like this:

![flower sprite](images/flower-sprite.png)

![blocks_1545308799_3392](images/blocks_1545308799_3392.png)
 
--- /task ---

Notice that your `draw flower`{:class="block3myblocks"} blocks now have a new input that is set to `1`: 

![blocks_1545308800_4787242](images/blocks_1545308800_4787242.png)

--- task ---

Change the numbers in the `draw flower`{:class="block3myblocks"} blocks so that the two flowers appear in different colours. You can pick any numbers between 0 and 200.

Your code should look similar to this:

![flower sprite](images/flower-sprite.png)

![blocks_1545308801_6151931](images/blocks_1545308801_6151931.png)

--- /task ---

--- task ---

Now add another input to set the size of the flower, so your `draw flower`{:class="block3myblocks"} block looks like this:

![flower sprite](images/flower-sprite.png)

![blocks_1545308802_7293386](images/blocks_1545308802_7293386.png)

With the block above, you can create flowers with different sizes:

![different sized flowers](images/flower-different-sizes.png)

--- hints ---

--- hint ---

Look at what you did to add the `colour` input, and repeat it to add a 'size' input that you can use to set the size of the Flower sprite. 

--- /hint ---

--- hint ---

Edit the `draw flower`{:class="block3myblocks"} block to add a new number input called 'size'.

You need to add the following block with a 'size' input to the `draw flower`{:class="block3myblocks"} definition block:

![blocks_1545308803_8389835](images/blocks_1545308803_8389835.png)

--- /hint ---

--- hint ---

Right-click on the `draw flower`{:class="block3myblocks"} definition block, click on **edit**, and add a number input called 'size'.

![flower sprite](images/flower-sprite.png)

Change your `define draw flower`{:class="block3myblocks"} script so it looks like this:

![blocks_1545308804_8986294](images/blocks_1545308804_8986294.png)

--- /hint ---

--- /hints ---

--- /task ---
--- task ---
In the `when green flag clicked`{:class="block3events"} script, change the second number in both `draw flower`{:class="block3myblocks"} blocks so that the two flowers appear in different sizes.

![blocks_1545308806_0463903](images/blocks_1545308806_0463903.png)
--- /task ---

--- task ---
Test your code to check whether the flowers have different sizes.
--- /task ---

--- task ---
It would be cool to choose the number of petals the flowers have.

Add another input so that you can draw flowers like this:

![flowers with different numbers of petals](images/flower-petals.png)

--- hints ---
--- hint ---

You need to add a 'petals' number input, and then use it in the `define draw flower`{:class="block3myblocks"} block. 

There are two places where you need to add the 'petals' input.

The number of degrees the Flower sprite should `turn`{:class="block3looks"} by is `360` divided by the number of petals. 

--- /hint ---

--- hint ---

Change your `define draw flower`{:class="block3myblocks"} block to look like this:

![flower sprite](images/flower-sprite.png)

![blocks_1545308807_1581116](images/blocks_1545308807_1581116.png)

Update your `repeat`{:class="block3control"} and `turn`{:class="block3looks"} blocks so they use the 'petals' input.

![blocks_1545308808_3068318](images/blocks_1545308808_3068318.png)

Update your `draw flower`{:class="block3myblocks"} blocks to use the 'petals' input.

![blocks_1545308809_4142375](images/blocks_1545308809_4142375.png)

--- /hint ---

--- hint ---

Edit your `define draw flower`{:class="block3myblocks"} block and add a new number input called 'petals'.

![flower sprite](images/flower-sprite.png)

Your code should look like this:

![blocks_1545308810_4962852](images/blocks_1545308810_4962852.png)

In the `when green flag clicked`{:class="block3events"} script, change the third number in both `draw flower`{:class="block3myblocks"} blocks so that the two flowers that appear have different numbers of petals.

![blocks_1545308811_6982303](images/blocks_1545308811_6982303.png)

--- /hint ---

--- /hints ---

--- /task ---

Next, edit your code so you can draw different flowers by pressing the <kbd>f</kbd> key. 

--- task ---

Now move your code for drawing flowers away from below the `when green flag clicked`{:class="block3events"} block, and put the code under a `when f key pressed`{:class="block3events"} block.

![flower sprite](images/flower-sprite.png)

![blocks_1545308812_8861165](images/blocks_1545308812_8861165.png)

![blocks_1545308814_005287](images/blocks_1545308814_005287.png)

--- /task ---

--- task ---

Press <kbd>f</kbd> to test your code. 

--- /task ---

--- task ---

Add more `draw flower`{:class="block3myblocks"} blocks to your program to draw flowers with different colours, sizes, and numbers of petals all over the Stage.

--- /task ---
