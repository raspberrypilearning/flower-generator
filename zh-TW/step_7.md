## 隨機花朵產生器

你將會使用你的`畫花朵` {：class =“ block3myblocks”}積木，在每次按下<kbd> r </kbd>時，出現一百朵隨機樣式的花在舞台上。

![random flowers](images/flower-random.png)

\--- task \---

Add a new Event block to your sprite's code so that `when the r key is pressed`{:class="block3events"}, the screen is `cleared`{:class="block3extensions"}.

![flower sprite](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

\--- /task \---

\--- task \---

Add in a `repeat`{:class="block3control"} block to go to a `random position`{:class="block3motion"} `100` times.

![flower sprite](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

\--- /task \---

\--- task \---

Use the `draw flower`{:class="block3myblocks"} block to create a flower that has a `random`{:class="block3operators"} colour between `0` and `199`.

You code should now look like this:

![flower sprite](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (100) (12) :: custom
end
```

\--- /task \---

This code creates one hundred flowers with different colours but with the same size and numbers of petals.

![flowers just with random colours](images/flower-random-colour.png)

\--- task \---

Can you modify the `when the r key is pressed`{:class="block3events"} script so the flowers' size and number of petals are also random?

\--- hints \---

\--- hint \---

The `draw flower`{:class="block3myblocks"} block should `pick random`{:class="block3operators"} numbers for the size and number of petals.

\--- /hint \---

\--- hint \---

The following blocks pick a random size between `50` and `150` and a random number of petals between `4` and `12`.

![flower sprite](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

\--- /hint \---

\--- hint \---

Your code should look like this:

![flower sprite](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

\--- /hint \---

\--- /hints \---

\--- /task \---

\--- task \---

Press <kbd>r</kbd> to see your random flowers.

\--- /task \---