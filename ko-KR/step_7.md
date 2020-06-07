## 랜덤하게 꽃 생성하기

이제 `꽃 그리기`{:class="block3myblocks"} 블럭을 사용하여 <kbd>r</kbd>키를 눌렀을 때 온 무대를 덮는 100개의 랜덤한 꽃을 만들어 볼 것입니다.

![랜덤한 꽃](images/flower-random.png)

\--- task \---

스프라이트의 코드에 새로운 이벤트 블록을 추가하여 `r 키를 눌렀을 때`{:class="block3events"} `모두 지우기`{:class="block3extensions"}가 되도록 합니다.

![꽃 스프라이트](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

\--- /task \---

\--- task \---

`반복하기`{:class="block3control"} 블럭을 추가하여 `무작위 위치로 이동하기`가 `100`번 일어나게 합니다.

![꽃 스프라이트](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

\--- /task \---

\--- task \---

`꽃 그리기`{:class="block3myblocks"} 블록을 사용하여 `0`과 `199` 사이의 `난수`{:class="block3operators"} 색을 가진 꽃을 그립니다.

다음과 같은 코드가 될 것입니다:

![꽃 스프라이트](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (100) (12) :: custom
end
```

\--- /task \---

이 코드는 색깔은 다르지만 크기와 꽃잎의 개수가 같은 100개의 꽃을 만듭니다.

![임의 색깔만 적용한 꽃](images/flower-random-colour.png)

\--- task \---

`r 키를 눌렀을 때`{:class="block3events"} 아래의 스크립트를 수정하여 꽃의 크기와 꽃잎의 개수도 랜덤하게 되도록 할 수 있나요?

\--- hints \---

\--- hint \---

`꽃 그리기`{:class="block3myblocks"} 블록은 꽃잎의 크기와 개수를 위한 `난수`를 골라야 합니다.

\--- /hint \---

\--- hint \---

다음 블록들은 `50`과 `150` 사이의 랜덤한 크기를 고르고 `4`와 `12` 사이의 랜덤한 꽃잎 개수를 고릅니다.

![꽃 스프라이트](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

\--- /hint \---

\--- hint \---

다음과 같은 코드가 될 것입니다:

![꽃 스프라이트](images/flower-sprite.png)

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

<kbd>r</kbd> 키를 눌러 랜덤한 꽃을 확인하세요.

\--- /task \---