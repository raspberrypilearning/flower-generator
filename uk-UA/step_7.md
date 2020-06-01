## Генератор випадкових квітів

Тепер ти використаєш свій блок `намалювати квітку`{:class="block3myblocks"}, щоб після того, як натиснуто <kbd>r</kbd>, створити сотні випадкових квітів по всій Сцені.

![випадкові квіти](images/flower-random.png)

\--- task \---

Додай новий блок з розділу Події до коду свого спрайта, щоб `коли клавішу r натиснуто`{:class="block3events"}, екран було `очищено`{:class="block3extensions"}.

![спрайт квітки](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

\--- /task \---

\--- task \---

Додай блок `повторити`{:class="block3control"}, щоб перейти до `випадкової позиції`{:class="block3motion"} `100` разів.

![спрайт квітки](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

\--- /task \---

\--- task \---

Використай блок `намалювати квітку`{:class="block3myblocks"}, щоб створити квітку, яка має `випадковий`{:class="block3operators"} колір від `0` до `199`.

Твій код має виглядати так:

![спрайт квітки](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (100) (12) :: custom
end
```

\--- /task \---

Цей код створює сотню квітів різних кольорів, але з однаковим розміром та кількістю пелюсток.

![квіти випадкових кольорів](images/flower-random-colour.png)

\--- task \---

Чи можеш ти змінити скрипт `коли клавішу r натиснуто`{:class="block3events"}, щоб розмір квітів та кількість пелюсток також була випадковою?

\--- hints \---

\--- hint \---

Блок `намалювати квітку`{:class="block3myblocks"} має містити `випадкові`{:class="block3operators"} числа для розміру та кількості пелюсток.

\--- /hint \---

\--- hint \---

Наступні блоки вибирають випадковий розмір між `50` та `150`, а також випадкову кількість пелюсток між `4` та `12`.

![спрайт квітки](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

\--- /hint \---

\--- hint \---

Твій код повинен виглядати так:

![спрайт квітки](images/flower-sprite.png)

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

Натисни <kbd>r</kbd>, щоб побачити свої випадкові квіти.

\--- /task \---