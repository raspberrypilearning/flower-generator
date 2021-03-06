## Генератор случайных цветов

Теперь мы будем использовать блок `нарисовать цветок`{:class="block3myblocks"}, чтобы создать сотню случайных цветов по всей Сцене, при нажатии <kbd>r</kbd>.

![случайные цветы](images/flower-random.png)

--- task ---

Добавь новый блок события в код твоего спрайта так, чтобы `когда клавиша r нажата`{:class="block3events"}, все `стиралось`{:class="block3extensions"} с экрана.

![спрайт цветка](images/flower-sprite.png)

```blocks3
когда клавиша [r v] нажата
стереть всё
```

--- /task ---

--- task ---

Добавь блок `повторить`{:class="block3control"}, чтобы перейти на `случайную позицию`{:class="block3motion"} `100` раз.

![спрайт цветка](images/flower-sprite.png)

```blocks3
повторить (100) раз 
  перейти на (случайное положение v)
end
```

--- /task ---

--- task ---

Используй блок `нарисовать цветок`{:class="block3myblocks"}, чтобы создать цветок, который будет `случайной`{:class="block3operators"} расцветки от `0` до `199`.

Твой код должен выглядеть так:

![спрайт цветка](images/flower-sprite.png)

```blocks3
когда клавиша [r v] нажата
стереть всё
повторить (100) раз 
  перейти на (случайное положение v)
  нарисовать цветок (выдать случайное от (0) до (199)) (100) (12) :: custom
end
```

--- /task ---

Код создаст сотню цветов разных расцветок, но одинакового размера и с одинаковым количеством лепестков.

![цветы только случайной расцветки](images/flower-random-colour.png)

--- task ---

Можешь ли ты изменить скрипт `когда клавиша [r v] нажата`{:class="block3events"} так, чтобы размер цветов и количество лепестков также были случайными?

--- hints ---


--- hint ---

Блок `нарисовать цветок`{:class="block3myblocks"} должен `выбрать случайные`{:class="block3operators"} числа для размера и количества лепестков.

--- /hint ---

--- hint ---

С помощью следующих блоков выбирается случайный размер между `50` и `150` и случайное количество лепестков между `4` и `12`.

![спрайт цветка](images/flower-sprite.png)

```blocks3
(выдать случайное от (50) до (150))

(выдать случайное от (4) до (12))
```

--- /hint ---

--- hint ---

Твой код должен выглядеть вот так:

![спрайт цветка](images/flower-sprite.png)

```blocks3
когда клавиша [r v] нажата
стереть всё
повторить (100) раз 
  перейти на (случайное положение v)
  нарисовать цветок (выдать случайное от (90) до (199)) (выдать случайное от (4) до (12)) :: custom
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

Нажми <kbd>r</kbd>, чтобы увидеть случайные цветы.

--- /task ---