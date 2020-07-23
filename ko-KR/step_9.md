## 도전 과제: 맞춤형 꽃 블록

이 꽃들은 모두 같은 수의 바깥 쪽 꽃잎과 안쪽 꽃잎을 가지고 있으며, 안쪽 꽃의 크기는 바깥 꽃에 비례합니다:

![스크린샷](images/flower-double-flowers.png)

이런 꽃은 `바깥쪽 색깔`, `안쪽 색깔`, `크기`를 입력으로 받는 `이중 꽃 그리기`{:class="block3myblocks"} 블록을 이용하여 만들 수 있습니다.

```blocks3
define 이중 꽃 그리기 (바깥쪽 색깔) (안쪽 색깔) (크기 :: custom-arg)
꽃 그리기 (바깥쪽 색깔 :: custom-arg) (크기 :: custom-arg) (12) :: custom
꽃 그리기 (안쪽 색깔 :: custom-arg) ((크기 :: custom-arg) / (2)) (20) :: custom
```

`이중 꽃 그리기`{:class="block3myblocks"} 블록은 같은 스타일로 많은 꽃을 그릴 수 있습니다:

```blocks3
when [d v] key pressed
erase all
go to x: (-100) y: (0)
이중 꽃 그리기 (160) (120) (100) :: custom
change x by (100)
이중 꽃 그리기 (120) (140) (75) :: custom
change x by (75)
이중 꽃 그리기 (140) (160) (50) :: custom
```

원하는 종류의 꽃을 만들기 위해 필요한 입력을 가진 나만의 블록을 만듭니다.

그런 다음 새로운 블록을 사용하여 멋진 디자인을 만들어봅시다!