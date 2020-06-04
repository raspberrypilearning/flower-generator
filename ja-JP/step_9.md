## チャレンジ：花を描くブロックをつくり直す

これらの花はすべて外側と内側の花びらの数が同じで、内側の花の大きさは外側の花の大きさに応じて変わります。

![スクリーンショット](images/flower-double-flowers.png)

このような花は引数に`外側の色`、`内側の色`、`大きさ`を引数に持つ独自の`八重咲きを描く`{:class="block3myblocks"}ブロックを使ってつくることができます。

```blocks3
define draw double flower (outer colour) (inner colour) (size :: custom-arg)
draw flower (outer colour :: custom-arg) (size :: custom-arg) (12) :: custom
draw flower (inner colour :: custom-arg) ((size :: custom-arg) / (2)) (20) :: custom
```

`八重咲きを描く`{:class="block3myblocks"}ブロックは同じ形式でたくさんの花を描（えが）くことができます：

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

Make a new custom block with the necessary inputs that you need to be able to change to create a type of flower that you like.

Then use your new block to create a cool design!