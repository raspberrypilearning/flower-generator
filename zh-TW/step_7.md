## 隨機花朵產生器

你將會使用你的`畫花朵`{:class="block3myblocks"}積木，在每次按下<kbd>r</kbd>時，出現一百朵隨機樣式的花在舞台上。

![隨機花朵](images/flower-random.png)

--- task ---

新增一個事件積木到角色的程式碼中，使`當r鍵被按下`{:class="block3events"}時, 會把舞台上的 `筆跡全部清除`{:class="block3extensions"}。

![花朵角色](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

--- /task ---

--- task ---

添加`重複`{:class="block3control"}`100`次積木和`定位到隨機位置`{:class="block3motion"}積木 ，使一百朵花會產生在隨機位置。

![花朵角色](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

--- /task ---

--- task ---

使用`畫花朵`{:class="block3myblocks"}積木，讓產生的花朵顏色在色彩碼`0`和`199`之間`隨機`{:class="block3operators"}挑選。

現在你的程式應該會像這樣：

![花朵角色](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  畫花朵 (pick random (0) to (199)) (100) (12) :: custom
end
```

--- /task ---

這個程式碼創造了一百種不同顏色的花，但是大小和花瓣數量卻是一樣的。

![只有顏色隨機的花朵](images/flower-random-colour.png)

--- task ---

你有辦法修改`當r鍵被按下`{:class="block3events"}的腳本，使花朵的大小和花瓣數也能隨機變化嗎？

--- hints ---


--- hint ---

`畫花朵`{:class="block3myblocks"}積木應該`隨機取數`{:class="block3operators"}來呈現大小和花瓣數。

--- /hint ---

--- hint ---

以下積木會隨機選擇`50`到`150`之間的大小，以及 `4`到`12`之間的花瓣數量 。

![花朵角色](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

--- /hint ---

--- hint ---

你的程式應該會像這樣：

![花朵角色](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  畫花朵 (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

按<kbd>r</kbd>看看你創造的隨機花朵。

--- /task ---