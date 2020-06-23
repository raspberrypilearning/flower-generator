## مولد زهور عشوائي

سوف تستخدم الآن تعليمة برمجية لــ`ارسم زهرة`{:class="block3myblocks"} لإنشاء مئات الزهور العشوائية في جميع أنحاء المرحلة كلما قمت بالضغط على <kbd>r</kbd>.

![أزهار عشوائية](images/flower-random.png)

--- task ---

أضف تعليمة برمجية جديدة من مجموعة الاحداث إلى تعليمة الكائن لخاص بك بحيث أن `عندما يتم الضغط على مفتاح r`{:class="block3events"}، تكون الشاشة`خالية`{:class="block3extensions"}.

![كائن الزهرة](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

--- /task ---

--- task ---

أضف في التعليمة `كرر`{:class="block3control"} للذهاب إلى `وضع عشوائي`{:class="block3motion"} `100` مرة.

![كائن الزهرة](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

--- /task ---

--- task ---

استخدم التعليمة البرمجية `رسم زهرة`{:class="block3myblocks"} لإنشاء زهرة لها لون `عشوائي`{:class="block3operators"} بين `0` و `199`.

يجب أن تبدو تعليماتك البرمجية على الشكل التالي:

![كائن الزهرة](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  رسم زهرة (pick random (0) to (199)) (100) (12) :: custom
end
```

--- /task ---

هذه التعليمات البرمجية تنشئ مائة زهرة بألوان مختلفة ولكن بنفس الحجم وأعداد الورق.

![الزهور فقط بألوان عشوائية](images/flower-random-colour.png)

--- task ---

هل يمكنك تعديل `عند الضغط على مفتاح r`{:class="block3events"} بحيث يكون حجم الزهور وعدد الورق البيضاء عشوائيًا أيضاً؟

--- hints ---


--- hint ---

التعليمة `رسم زهرة`{:class="block3myblocks"} يجب أن `تختار أرقام عشوائية `{:class="block3operators"} لحجم وعدد الورق.

--- /hint ---

--- hint ---

التعليمة التالية تختار حجم عشوائي بين `50` و `150` وعدد عشوائي من الورق بين `4` و `12`.

![كائن الزهرة](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

--- /hint ---

--- hint ---

يجب أن تبدو التعليمات البرمجية خاصتك بالشكل التالي:

![كائن الزهرة](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  رسم زهرة (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

اضغط على <kbd>r</kbd> لرؤية زهورك العشوائية.

--- /task ---