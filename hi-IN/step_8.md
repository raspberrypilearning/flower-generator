## फूल के पैटर्न

फूलों के साफ-सुथरे पैटर्न बनाने के लिए आप अपने `draw flower`{:class="block3myblocks"} ब्लॉक का भी उपयोग कर सकते हैं।

\--- task \---

अपनी पसंद का कोई फूल या फूलों का संयोजन बनाएँ। यहाँ एक उदाहरण है:

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
when [p v] key pressed
erase all
go to x: (-150) y: (100)
draw flower (150) (80) (7) :: custom
draw flower (130) (35) (20) :: custom
```

\--- /task \---

\--- task \---

अपने फूल को देखने के लिए <kbd>p</kbd> दबाएँ। उदाहरण इस तरह दिखता है:

![फूल का पैटर्न](images/flower-for-pattern-example.png)

\--- /task \---

इससे पहले कि आप अपना पैटर्न बना सकें, आपको स्टेज पर किन्हीं बचे हुए फूलों को साफ कर देना चाहिए।

\--- task \---

Pen (पेन) टैब में `erase all` ब्लॉक पर क्लिक करें।

```blocks3
सभी मिटाएँ
```

\--- /task \---

\--- task \---

फूल स्प्राइट पर राइट-क्लिक करें और इसे `hide`{:class="block3looks"} करें ताकि यह स्टेज पर दिखाई न दे। (आप स्प्राइट को फिर से `show`{:class="block3looks"} कर सकते हैं यदि आपको यह देखने की जरूरत पड़े कि यह कहाँ पर है।)

\--- /task \---

\--- task \---

अब स्टेज पर ऊपर की तरफ इन फूलों की एक पंक्ति बनाएँ। यहाँ एक उदाहरण कोड है, जिसमें आपको संख्याओं को समायोजित करने की जरूरत पड़ सकती है ताकि यह आपके फूल के साथ काम कर सके:

![फूल स्प्राइट](images/flower-sprite.png)

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

फूलों की पंक्ति को देखने के लिए `p` दबाएँ।

![एक पंक्ति में 4 फूल](images/flower-pattern-row-example.png)

\--- /task \---

\--- task \---

फूलों की अधिक पंक्तियाँ बनाने के लिए एक और लूप जोड़ें। यह उदाहरण तीन पंक्तियाँ बनाने के लिए एक `repeat 3`{:class="block3control"} लूप जोड़ता है।

![फूल स्प्राइट](images/flower-sprite.png)

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

फूलों का एक ग्रिड बनाने के लिए <kbd>p</kbd> दबाएँ:

![फूलों की एक 4 x 4 ग्रिड](images/flower-pattern-rows-example.png)

\--- /task \---

क्या आप फूलों को बनाने की गति को तेज़ करना चाहते हैं?

\--- task \---

Right-click on the `draw flower`{:class="block3myblocks"} definition block and then click on **edit**. Click on the **Run without screen refresh** box.

![turn no refresh option off](images/flower-no-refresh.png)

Now the flowers get drawn more quickly.

\--- /task \---

You can also change the colour of the Stage.

\--- task \---

Click on **Choose a backdrop**, and then click on **Paint**. Create an orange backdrop by using the Fill tool in Bitmap mode.

![paint new backdrop](images/flower-orange-backdrop.png)

If you use orange for the backdrop and the Flower sprite, then the numbers for different colours will match for the sprite and the backdrop.

\--- /task \---

\--- task \---

Now you can use the `set colour effect`{:class="block3looks"} on the Stage to change the colour of the backdrop.

![stage sprite](images/stage-sprite.png)

```blocks3
when [p v] key pressed
set [color v] effect to (30)
```

\--- /task \---

\--- task \---

Try to create a pattern you like.

Here's an example:

![flowers on a green background](images/flower-pattern-background.png)

\--- /task \---

When you put it all together, you can create an amazing effect:

![animation of lots of flowers](images/flower-gen-example.gif)