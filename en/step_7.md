## Random flower generator

Create a hundred random flowers all over the Stage when you press the <kbd>r</kbd> key.

![Lots of flowers in different shapes, sizes and positions](images/flower-random.png)

--- task ---

Add a new Event block to your sprite's code so that `when the r key is pressed`{:class="block3events"}, the screen is `cleared`{:class="block3extensions"}.

![flower sprite](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

--- /task ---

--- task ---

Add in a `repeat`{:class="block3control"} block to go to a `random position`{:class="block3motion"} `100` times.

![flower sprite](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

--- /task ---


--- task ---

Use the `draw flower`{:class="block3myblocks"} block to create a flower that has a `random`{:class="block3operators"} colour between `0` and `199`.

You code should now look like this:

![flower sprite](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  +draw flower (pick random (0) to (199)) (100) (12) :: custom
end
```

--- /task ---

--- task ---

Press <kbd>r</kbd> to see your random flowers.

--- /task ---

This code creates one hundred flowers with different colours but with the same size and numbers of petals. 

![Multiple flowers of the same size and number of petals, but with random colours](images/flower-random-colour.png)

--- task ---

Change your code so that the size and the number of petals is also a randomly chosen number.

![flower sprite](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

--- /task ---


