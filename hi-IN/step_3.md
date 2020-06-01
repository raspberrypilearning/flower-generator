## फूल बनाने के लिए एक कस्टम ब्लॉक बनाएँ

यदि आप बहुत सारे फूल बनाना चाहते हैं तो क्या करना होगा? कोड की बहुत सारी प्रतियाँ बनाने के बजाय, आप Scratch में अपना ब्लॉक बनाएँगे और हर बार जब आप फूल बनाना चाहते हैं तो इसका उपयोग करेंगे।

\--- task \---

'फूल बनाएँ' नामक अपना ब्लॉक बनाने के लिए **My Blocks** (मेरे ब्लॉक) पर क्लिक करें और फिर **Make a Block** (ब्लॉक बनाएँ) पर।

![स्क्रीनशॉट](images/flower-make-block.png)

\--- /task \---

\--- task \---

**More blocks** (अधिक ब्लॉक) खंड में, अब `draw flower`{:class="block3myblocks"} (फूल बनाएँ) नामक एक नया ब्लॉक है, और स्टेज पर एक नया परिभाषा ब्लॉक।

```blocks3
draw flower :: custom

define draw flower
```

\--- /task \---

\--- task \---

`when green flag clicked`{:class="block3events"} ब्लॉक से फूल बनाने के लिए अपने कोड को नए `draw flower`{:class="block3myblocks"} definition block (परिभाषा ब्लॉक) में ले जाएँ।

आपका कोड इस प्रकार दिखना चाहिए:

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
define draw flower
repeat (6) 
  stamp
  turn cw (60) degrees
end

when green flag clicked
```

\--- /task \---

\--- task \---

स्टेज को खाली करने और जब हरे झंडे को क्लिक किया जाता है तो अपने नए `draw flower`{:class="block3myblocks"} ब्लॉक का उपयोग करने के लिए निम्न कोड जोड़ें:

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
draw flower :: custom
```

\--- /task \---

\--- task \---

अपने कोड का परीक्षण करने और यह जाँच करने के लिए हरे झंडे पर क्लिक करें कि क्या आपको फूल दिखाई देता है।

\--- /task \---

\--- task \---

अब स्प्राइट को दूसरी जगह ले जाने और दूसरा फूल बनाने के लिए अपना कोड बदलें:

![फूल स्प्राइट](images/flower-sprite.png)

```blocks3
when green flag clicked
erase all
go to x: (75) y: (75)
draw flower :: custom
go to x: (-75) y: (-75)
draw flower :: custom 
```

\--- /task \---

\--- task \---

यह जाँच करने के लिए अपने कोड का परीक्षण करें कि अब आपको दो फूल दिखाई देते हैं।

![स्क्रीनशॉट](images/flower-two.png)

\--- /task \---