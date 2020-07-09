## Random फूल जनरेटर

अब आप जब भी <kbd>r</kbd> को दबाएँगे तो पूरे स्टेज पर सौ यादृच्छिक फूल बनाने के लिए अपने `draw flower`{:class="block3myblocks"} ब्लॉक का उपयोग करेंगे।

![यादृच्छिक फूल](images/flower-random.png)

\--- task \---

अपने स्प्राइट कोड में एक नया इवेंट ब्लॉक जोड़ें ताकि `when the r key is pressed`{:class="block3events"} से, स्क्रीन `cleared`{:class="block3extensions"} साफ़ हो जाए।

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
```

\--- /task \---

\--- task \---

`random position`{:class="block3motion"} पर `100` बार जाने के लिए एक `repeat`{:class="block3control"} ब्लॉक जोड़ें।

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
repeat (100)
  go to (random position v)
end
```

\--- /task \---

\--- task \---

एक ऐसा फूल बनाने के लिए जिसका `0` और `199` के बीच कोई `random`{:class="block3operators"} यादृच्छिक रंग हो `draw flower`{:class="block3myblocks"} ब्लॉक का उपयोग करें।

आपका कोड अब इस प्रकार दिखना चाहिए:

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
when [r v] key pressed
erase all
repeat (100) 
  go to (random position v)
  draw flower (pick random (0) to (199)) (100) (12) :: custom
end
```

\--- /task \---

यह कोड अलग-अलग रंगों वाले एक सौ फूल बनाता है लेकिन उनका आकार और पंखुड़ियों की संख्या समान होती है।

![केवल यादृच्छिक रंगों के साथ फूल](images/flower-random-colour.png)

\--- task \---

क्या आप `when the r key is pressed`{:class="block3events"} स्क्रिप्ट को संशोधित कर सकते हैं ताकि फूलों का आकार और पंखुड़ियों की संख्या भी यादृच्छिक हो?

\--- hints \---

\--- hint \---

`draw flower`{:class="block3myblocks"} ब्लॉक को आकार और पंखुड़ियों की संख्या के लिए `pick random`{:class="block3operators"} यादृच्छिक संख्याएँ चुननी चाहिए।

\--- /hint \---

\--- hint \---

निम्नलिखित ब्लॉक `50` और `150` के बीच का कोई यादृच्छिक आकार और `4` और `12` के बीच की पंखुड़ियों की कोई यादृच्छिक संख्या चुनते हैं।

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
(pick random (50) to (150))

(pick random (4) to (12))
```

\--- /hint \---

\--- hint \---

आपका कोड इस प्रकार दिखना चाहिए:

![फूल स्प्राइट](images/flower-sprite.png)

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

अपने यादृच्छिक (random) फूलों को देखने के लिए <kbd>r</kbd> दबाएँ।

\--- /task \---