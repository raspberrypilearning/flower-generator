## Завдання: власні блоки для квітів

Ці квіти мають однакову кількість зовнішніх та внутрішніх пелюсток, а розмір внутрішньої квітки складає певну частину від розміру зовнішньої:

![знімок екрана](images/flower-double-flowers.png)

Ти можеш створювати подібні квіти за допомогою власного блоку `намалювати подвійну квітку`{:class="block3myblocks"} з параметрами `зовнішній колір`, `внутрішній колір` та `розмір`:

```blocks3
define draw double flower (outer colour) (inner colour) (size :: custom-arg)
draw flower (outer colour :: custom-arg) (size :: custom-arg) (12) :: custom
draw flower (inner colour :: custom-arg) ((size :: custom-arg) / (2)) (20) :: custom
```

Блок `намалювати подвійну квітку`{:class="block3myblocks"} може малювати велику кількість квітів такого виду:

```blocks3
when [d v] key pressed
erase all
go to x: (-100) y: (0)
draw double flower (160) (120) (100) :: custom
change x by (100)
draw double flower (120) (140) (75) :: custom
change x by (75)
draw double flower (140) (160) (50) :: custom
```

Створи новий власний блок з необхідними параметрами, які можна змінювати для створення бажаних квітів.

Потім використай свій новий блок для створення класних малюнків!