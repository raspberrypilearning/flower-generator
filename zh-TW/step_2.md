## 創造一朵花

首先，創造一朵可以在場景上繪製的花朵。

\--- task \---

新建一個新的Scratch專案，然後刪除貓咪角色。

[[[generic-scratch3-new-project]]]

\--- /task \---

\--- task \---

把畫筆這個擴充功能添加到專案裡。

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

現在使用"繪畫"工具來創造形狀如同花瓣的新角色。

點擊**選擇角色** ，接著點擊**繪畫**並將角色重新命名為“花朵”。

[[[generic-scratch3-draw-sprite]]]

\--- /task \---

\--- task \---

使用圓形工具來畫出一個橘色的實心花瓣形狀。

![screenshot](images/flower-petal.png)

Later, you will use code to add more colour.

\--- /task \---

\--- task \---

Add the following code to the Flower sprite to `stamp`{:class="block3extensions"} a flower with six equally rotated petals `when the green flag is clicked`{:class="block3control"}.

![screenshot](images/flower-6-straight.png)

```blocks3
when green flag clicked
repeat (6) 
  stamp
  turn cw (60) degrees
end
```

\--- /task \---

You may find that your petals are arranged in an odd way:

![screenshot](images/flower-6-offset.png)

This is because the sprite is being rotated around its centre.

\--- task \---

Move your petal so its bottom is in the centre.

![screenshot](images/flower-crosshair-annotated.png)

Doing this may be easier if you zoom out.

\--- /task \---

Before you run your code again, you should `erase all`{:class="block3extensions"} the sprites on the Stage to clear it.

\--- task \---

Click on the `erase all` block in the Pen blocks section.

```blocks3
erase all
```

\--- /task \---

\--- task \---

Run your code again to check that the flower's petals are straight now.

![screenshot](images/flower-6-straight.png)

If not, adjust the petal's position until its bottom in the centre.

\--- /task \---