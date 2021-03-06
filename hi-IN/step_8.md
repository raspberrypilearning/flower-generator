## फूल के पैटर्न

फूलों के साफ-सुथरे पैटर्न बनाने के लिए आप अपने `draw flower`{:class="block3myblocks"} ब्लॉक का भी उपयोग कर सकते हैं।

--- task ---

अपनी पसंद का कोई फूल या फूलों का संयोजन बनाएँ। यहाँ एक उदाहरण है:

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
when [p v] key pressed
erase all
go to x: (-150) y: (100)
draw flower (150) (80) (7) :: custom
draw flower (130) (35) (20) :: custom
```

--- /task ---

--- task ---

अपने फूल को देखने के लिए <kbd>p</kbd> दबाएँ। उदाहरण इस तरह दिखता है:

![फूल का पैटर्न](images/flower-for-pattern-example.png)

--- /task ---

इससे पहले कि आप अपना पैटर्न बना सकें, आपको स्टेज पर किन्हीं बचे हुए फूलों को साफ कर देना चाहिए।

--- task ---

Pen (पेन) टैब में `erase all` ब्लॉक पर क्लिक करें।

```blocks3
erase all
```

--- /task ---

--- task ---

फूल स्प्राइट पर राइट-क्लिक करें और इसे `hide`{:class="block3looks"} करें ताकि यह स्टेज पर दिखाई न दे। (आप स्प्राइट को फिर से `show`{:class="block3looks"} कर सकते हैं यदि आपको यह देखने की जरूरत पड़े कि यह कहाँ पर है।)

--- /task ---

--- task ---

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

--- /task ---

--- task ---

फूलों की पंक्ति को देखने के लिए `p` दबाएँ।

![एक पंक्ति में 4 फूल](images/flower-pattern-row-example.png)

--- /task ---

--- task ---

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

--- /task ---

--- task ---

फूलों का एक ग्रिड बनाने के लिए <kbd>p</kbd> दबाएँ:

![फूलों की एक 4 x 4 ग्रिड](images/flower-pattern-rows-example.png)

--- /task ---

क्या आप फूलों को बनाने की गति को तेज़ करना चाहते हैं?

--- task ---

`draw flower`{:class="block3myblocks"} परिभाषा ब्लॉक पर राइट-क्लिक करें और फिर **edit** पर क्लिक करें। **स्क्रीन रिफ्रेश किए बिना चलाएं** बॉक्स पर क्लिक करें।

![कोई ताज़ा विकल्प बंद न करें](images/flower-no-refresh.png)

अब फूल अधिक तेज़ी से खींचे जाते हैं।

--- /task ---

आप स्टेज का रंग भी बदल सकते हैं

--- task ---

**एक पृष्ठभूमि चुनें** पर क्लिक करें, और फिर **पेंट** पर क्लिक करें। बिटमैप मोड में भरण उपकरण का उपयोग करके एक नारंगी पृष्ठभूमि बनाएं।

![नई पृष्ठभूमि पेंट करें](images/flower-orange-backdrop.png)

यदि आप बैकड्रॉप और फ्लावर स्प्राइट के लिए नारंगी का उपयोग करते हैं, तो विभिन्न रंगों के लिए नंबर स्प्राइट और बैकड्रॉप के लिए मेल खाएंगे।

--- /task ---

--- task ---

अब आप बैकड्रॉप के रंग को बदलने के लिए स्टेज पर `set colour effect`{:class="block3looks"} का उपयोग कर सकते हैं

![स्टेज स्प्राइट](images/stage-sprite.png)

```blocks3
when [p v] key pressed
set [color v] effect to (30)
```

--- /task ---

--- task ---

अपनी पसंद का पैटर्न बनाने की कोशिश करें।

यहाँ एक उदाहरण है:

![हरे रंग की पृष्ठभूमि पर फूल](images/flower-pattern-background.png)

--- /task ---

जब आप यह सब एक साथ रखते हैं, तो आप एक अद्भुत प्रभाव बना सकते हैं:

![बहुत सारे फूलों का एनीमेशन](images/flower-gen-example.gif)