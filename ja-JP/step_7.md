## ランダムに花をつくりだす

`花を描く`{:class="block3myblocks"}ブロックを、<kbd>r</kbd>キーを押すたびにステージ全体にランダムに100本の花をつくるのに使えます。

![ランダムな花](images/flower-random.png)

--- task ---

新しくイベントブロックを追加して、`rキーが押されたとき`{:class="block3events"}に、スクリーンを`全部消す`{:class="block3events"}ようにします。

![花のスプライト](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

--- /task ---

--- task ---

`繰り返す`{:class="block3control"}ブロックを追加し、`どこかの場所へ行く`{:class="block3motion"}を`100回`繰り返すようにします。

![花のスプライト](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

--- /task ---

--- task ---

`花を描く`{:class="block3myblocks"}ブロックを使って、`0`から`199`までの`ランダム`{:class="block3operators"}な色になっている花をつくります。

コードは以下のようになります：

![花のスプライト](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  花を描く (pick random (0) to (199)) (100) (12) :: custom
end
```

--- /task ---

このプログラムでは、いろんな色で100個の花をつくりますが、大きさと花びらの数は同じです。

![ランダムな色だけの花](images/flower-random-colour.png)

--- task ---

`rキーを押したとき`{:class="block3events"}のスクリプトを変更して、花の大きさや花びらの数もランダムにできますか？

--- hints ---


--- hint ---

`花を描く`{:class="block3myblocks"}ブロックは、大きさや花びらの数を`乱数`{:class="block3operators"}にしなければなりません。

--- /hint ---

--- hint ---

次のブロックは大きさを`50`から`150`までのランダムな大きさに、花びらの数を`4`から`12`のランダムな枚数にします。

![花のスプライト](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

--- /hint ---

--- hint ---

コードは次のようになります：

![花のスプライト](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  花を描く (pick random (0) to (199)) (pick random (50) to (150)) (pick random (4) to (12)) :: custom
end
```

--- /hint ---

--- /hints ---

--- /task ---

--- task ---

<kbd>r</kbd>キーを押すとランダムに花が表示されます。

--- /task ---