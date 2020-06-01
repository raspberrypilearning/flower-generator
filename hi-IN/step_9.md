## चुनौती: कस्टम फूल ब्लॉक

इन सभी फूलों में बाहरी और आंतरिक पंखुड़ियों की संख्या समान होती है, और आंतरिक फूल का आकार बाहरी फूल के अनुपात में होता है:

![स्क्रीनशॉट](images/flower-double-flowers.png)

आप इस तरह के फूल `draw double flower`{:class="block3myblocks"} कस्टम ब्लॉक की मदद से बना सकते हैं जिसमें `outer colour`, `inner colour`, और `size` के लिए इनपुट होती हैं:

```blocks3
define draw double flower (outer colour) (inner colour) (size :: custom-arg)
draw flower (outer colour :: custom-arg) (size :: custom-arg) (12) :: custom
draw flower (inner colour :: custom-arg) ((size :: custom-arg) / (2)) (20) :: custom
```

इस `draw double flower`{:class="block3myblocks"} ब्लॉक से एक ही शैली में बहुत सारे फूल बनाए जा सकते हैं:

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

आवश्यक इनपुट के साथ एक नया कस्टम ब्लॉक बनाएँ, जिसे आप उस तरह के फूल बनाने के लिए बदल सकें जिस तरह के आपको पसंद हों।

फिर अपने नए ब्लॉक का उपयोग एक बढ़िया डिजाइन बनाने के लिए करें!