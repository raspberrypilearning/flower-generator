## 挑戰：客製花朵積木

這些花的外花瓣和內花瓣數量都一樣，而且內花朵和外花朵的大小成比例：

![截圖](images/flower-double-flowers.png)

你可以創造一個有`外部顏色` ，`內部顏色`和`大小`輸入的 `畫雙花`{:class="block3myblocks"}的客製積木，來畫出這些花：

```blocks3
define 畫雙花 (外部顏色) (內部顏色) (大小 :: custom-arg)
畫花朵 (外部顏色 :: custom-arg) (大小 :: custom-arg) (12) :: custom
畫花朵 (內部顏色 :: custom-arg) ((大小 :: custom-arg) / (2)) (20) :: custom
```

`畫雙花`{:class="block3myblocks"}積木可以繪製許多相同樣式的花朵：

```blocks3
when [d v] key pressed
erase all
go to x: (-100) y: (0)
畫雙花 (160) (120) (100) :: custom
change x by (100)
畫雙花 (120) (140) (75) :: custom
change x by (75)
畫雙花 (140) (160) (50) :: custom
```

創建一個客製積木並設定你想要變更的輸入，來畫出你喜歡的花朵類型。

然後使用你的新積木來創造一個很酷的設計吧！