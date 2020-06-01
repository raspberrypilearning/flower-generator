## مولد زهور عشوائي

سوف تستخدم الآن تعليمة برمجية لــ`ارسم زهرة`{:class="block3myblocks"} لإنشاء مئات الزهور العشوائية في جميع أنحاء المرحلة كلما قمت بالضغط على <kbd>r</kbd>.

![random flowers](images/flower-random.png)

\--- task \---

أضف تعليمة برمجية جديدة من مجموعة الاحداث إلى تعليمة الكائن لخاص بك بحيث أن `عندما يتم الضغط على مفتاح r `{:class="block3events"}، تكون الشاشة`خالية`{:class="block3extensions"}.

![flower sprite](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

\--- /task \---

\--- task \---

أضف في التعليمة `كرر`{:class="block3control"} للذهاب إلى `وضع عشوائي`{:class="block3motion"} `100` مرة.

![flower sprite](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

\--- /task \---

\--- task \---

استخدم التعليمة البرمجية `رسم زهرة`{:class="block3myblocks"} لإنشاء زهرة لها لون `عشوائي`{:class="block3operators"} بين `0` و `199`.

يجب أن تبدو تعليماتك البرمجية على الشكل التالي:

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

هذه التعليمات البرمجية تنشئ مائة زهرة بألوان مختلفة ولكن بنفس الحجم وأعداد الورق.

![flowers just with random colours](images/flower-random-colour.png)

\--- task \---

هل يمكنك تعديل `عند الضغط على مفتاح r`{:class="block3events"} بحيث يكون حجم الزهور وعدد الورق البيضاء عشوائيًا أيضاً؟

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