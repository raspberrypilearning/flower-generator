## 花朵圖案

你還可以使用你的`畫花朵` {：class =“ block3myblocks”}積木創造出整齊的花朵圖案。

\--- task \---

創造一個你喜歡的花朵或花朵組合。 範例如下：

![flower sprite](images/flower-sprite.png)

```blocks3
when [p v] key pressed
erase all
go to x: (-150) y: (100)
draw flower (150) (80) (7) :: custom
draw flower (130) (35) (20) :: custom
```

\--- /task \---

\--- task \---

按<kbd> p </kbd>看看你創造的花朵。 範例看起來如下：

![a flower pattern](images/flower-for-pattern-example.png)

\--- /task \---

在創造圖案之前，應清除所有留在舞台上的花朵。

\--- task \---

點擊畫筆欄位的 `筆跡全部清除` 積木。

```blocks3
erase all
```

\--- /task \---

\--- task \---

在花朵角色上點擊右鍵並` 隱藏 ` {：class =“ block3looks”}它，這樣它就不會出現在舞台上。 （如果需要查看角色，你可以`顯示` {：class =“ block3looks”}角色。）

\--- /task \---

\--- task \---

現在在舞台上方繪製一排花。 這裡有一些範例程式碼，你可能需要調整數字，讓它能配合你的花朵：

![flower sprite](images/flower-sprite.png)

```blocks3
when [p v] key pressed
erase all
go to x: (-150) y: (100)
repeat (4) 
  draw flower (150) (80) (7) :: custom
  draw flower (130) (35) (20) :: custom
  change x by (100)
end
```

\--- /task \---

\--- task \---

按` p `看看你創造的一排花朵。

![4 flowers in a row](images/flower-pattern-row-example.png)

\--- /task \---

\--- task \---

新增一個迴圈來創造更多排花朵。 這個範例會新增 `重複3次`{:class="block3control"} 的迴圈來畫出三排花朵。

![flower sprite](images/flower-sprite.png)

```blocks3
when [p v] key pressed
erase all
go to x: (-150) y: (100)
repeat (3) 
  repeat (4) 
    draw flower (150) (80) (7) :: custom
    draw flower (130) (35) (20) :: custom
    change x by (100)
  end
  set x to (-150)
  change y by (-100)
end
```

\--- /task \---

\--- task \---

按<kbd> p </kbd>來畫出網格狀排列花朵。

![a 4 x 4 grid of flowers](images/flower-pattern-rows-example.png)

\--- /task \---

想要加快畫花的速度嗎？

\--- task \---

在`畫花朵` {：class =“ block3myblocks”}定義積木上點擊右鍵並選擇**編輯 ** ： 勾選 **執行完畢再更新畫面**。

![turn no refresh option off](images/flower-no-refresh.png)

現在花畫得更快了。

\--- /task \---

你還可以更改舞台的顏色。

\--- task \---

點擊**選個背景** ，然後單擊** 繪畫 ** 。 Create an orange backdrop by using the Fill tool in Bitmap mode.

![paint new backdrop](images/flower-orange-backdrop.png)

If you use orange for the backdrop and the Flower sprite, then the numbers for different colours will match for the sprite and the backdrop.

\--- /task \---

\--- task \---

Now you can use the `set colour effect`{:class="block3looks"} on the Stage to change the colour of the backdrop.

![stage sprite](images/stage-sprite.png)

```blocks3
when [p v] key pressed
set [color v] effect to (30)
```

\--- /task \---

\--- task \---

Try to create a pattern you like.

Here's an example:

![flowers on a green background](images/flower-pattern-background.png)

\--- /task \---

When you put it all together, you can create an amazing effect:

![animation of lots of flowers](images/flower-gen-example.gif)