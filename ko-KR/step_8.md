## 꽃 패턴 그리기

`꽃 그리기`{:class="block3myblocks"} 블록을 사용하여 근사한 꽃 패턴을 만들 수도 있습니다.

\--- task \---

꽃이나 원하는 꽃의 조합을 만들어봅시다. 아래 예제를 참고하세요:

![꽃 스프라이트](images/flower-sprite.png)

```blocks3
when [p v] key pressed
erase all
go to x: (-150) y: (100)
draw flower (150) (80) (7) :: custom
draw flower (130) (35) (20) :: custom
```

\--- /task \---

\--- task \---

<kbd>p</kbd>를 눌러 꽃을 확인하세요. 그러면 다음과 같이 보일 것입니다:

![꽃 패턴](images/flower-for-pattern-example.png)

\--- /task \---

패턴을 만들려면 먼저 무대에서 남은 꽃을 지워야 합니다.

\--- task \---

펜 블록 영역에 있는 `모두 지우기` 블럭을 누릅니다.

```blocks3
erase all
```

\--- /task \---

\--- task \---

꽃 스프라이트를 마우스 오른쪽 버튼으로 클릭하고 `숨기기`{:class="block3looks"} 를 눌러 무대에 표시되지 않도록 합니다. (어디 있는지 확인해야 한다면 `보이기`{:class="block3looks"}를 눌러 스프라이트를 다시 보이게 할 수 있습니다.)

\--- /task \---

\--- task \---

이제 무대 상단에 꽃들의 행을 그립니다. 다음은 예제 코드입니다(숫자를 조정해야 할 수도 있습니다):

![꽃 스프라이트](images/flower-sprite.png)

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

`p` 키를 눌러 꽃을 확인하세요:

![한 행에 놓인 4개의 꽃](images/flower-pattern-row-example.png)

\--- /task \---

\--- task \---

더 많은 꽃 행을 만들려면 다른 반복을 추가하세요. 다음 예시는 `3번 반복하기`{:class="block3control"} 블록을 추가하여 3개의 행을 만듭니다:

![꽃 스프라이트](images/flower-sprite.png)

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

<kbd>p</kbd> 키를 눌러 꽃으로 된 격자를 확인하세요:

![4 x 4 꽃 격자](images/flower-pattern-rows-example.png)

\--- /task \---

꽃 그리기 속도를 높이고 싶나요?

\--- task \---

`꽃 그리기`{:class="block3myblocks"} 정의하기 블록을 우클릭하고 **편집**을 클릭합니다. **화면을 새로고침 없이 실행하기**를 클릭하세요.

![새로 고침 안함 옵션 끄기](images/flower-no-refresh.png)

이제 꽃이 더 빨리 그려집니다.

\--- /task \---

무대의 색상을 변경할 수도 있습니다.

\--- task \---

**배경 고르기**를 클릭한 다음 **그리기**를 클릭합니다. 비트맵 모드에서 채우기 도구를 사용하여 주황색 배경을 만듭니다.

![새로운 배경 그리기](images/flower-orange-backdrop.png)

배경과 꽃 스프라이트에 둘 다 주황색을 사용하면 색깔을 나타내는 숫자가 배경과 꽃 스프라이트에서 일치할 것입니다.

\--- /task \---

\--- task \---

이제 무대에서 `색깔 효과 정하기`{:class="block3looks"} 블록을 이용하여 배경의 색깔을 바꿀 수 있습니다.

![무대 스프라이트](images/stage-sprite.png)

```blocks3
when [p v] key pressed
set [color v] effect to (30)
```

\--- /task \---

\--- task \---

원하는 패턴을 만들어보세요.

아래 예제를 참고하세요:

![녹색 배경에 놓인 꽃](images/flower-pattern-background.png)

\--- /task \---

모든 작업을 마치면 재미있는 효과를 얻을 수 있습니다:

![꽃 애니메이션](images/flower-gen-example.gif)