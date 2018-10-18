## Random flower generator

You will now use your `draw flower`{:class="blockmoreblocks"} block to create a 100 random flowers all over the stage when you press `r`.

![random flowers](images/flower-random.png)

--- task ---

Add a new Event block to your code so that `when the r key is pressed`{:class="blockevents"} the screen is `cleared`{:class="blockpen"}.

```blocks
when [r v] key pressed
clear
```

--- /task ---

--- task ---

Add in a `repeat`{:class="blockcontrol"} block to go to a `random position`{:class="blockmotion"} `100` times.

```blocks
repeat (100)
  go to [random position v]
end
```

--- /task ---

--- task ---

Use the `draw flower`{:class="blockmoreblocks"} block to create a flower which will have a `random`{:class="blockoperators"} colour between `0` and `199`.

You code should now look like this:

```blocks
when [r v] key pressed
clear
repeat (100) 
  go to [random position v]
  draw flower (pick random (0) to (199)) (100) (12) :: custom
end
```

--- /task ---

This code will create 100 flowers with different colours but all with the same size and numbers of petals. 

![flowers just with random colours](images/flower-random-colour.png)

--- task ---

Can you modify your program so the size and number of petals is also random?

--- hints ---

--- hint ---

The `draw flower`{:class="blockmoreblocks"} block should `pick random`{:class="blockoperators"} numbers for the size and number of petals.

--- /hint ---

--- hint ---

The following blocks will pick a random size between `50` and `150` and between `4` and `12` for the number of petals.

```blocks
(pick random (50) to (150))

(pick random (4) to (12))
```

--- /hint ---

--- hint ---

Your code should look like this:

```blocks
when [r v] key pressed
clear
repeat (100) 
  go to [random position v]
  draw flower (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

--- /hint ---

--- /hints ---

--- /task ---



