## एक हेड रोल व्यायाम जोड़ें

अब जब आप प्रत्येक व्यायाम को दोहराने की संख्या को नियंत्रित कर सकते हैं, तो यह दूसरा व्यायाम दिनचर्या जोड़ने का समय है।

--- task ---

इस व्यायाम के लिए, आप `say`{:class="block3looks"} की जगह `Text to Speech`{:class="block3extensions"} का उपयोग करेंगे ताकि कंप्यूटर द्वारा व्यायाम निर्देश बोले जा सकें।

Scratch विंडो के निचले बाएं कोने में **Add Extension** बटन पर क्लिक करें

![एक्सटेंशन बटन](images/extensionsButton.png)

**Text to Speech** एक्सटेंशन चुनें।

![टेक्स्ट टू स्पीच एक्सटेंशन](images/textToSpeechExtension.png)

`Text to Speech`{:class="block3extensions"} ब्लॉक का एक नया सेट दिखाई देगा।

![Text to Speech (लिखे हुए को बोलने में बदलना) ब्लॉक](images/textToSpeechBlocks.png)

--- /task ---

इसके बाद, आप कोड के एक अलग ब्लॉक के रूप में हेड रोल व्यायाम बनाएंगे, जिसे आप अंत में अपने मुख्य कोड में जोड़ देंगे।

--- task ---

**Nadia** स्प्राइट चुनें और `repeat`{:class="block3control"} ब्लॉक चुनें।

दोहराव की संख्या को नियंत्रित करने के लिए `Variables`{:class="block3variables"} ब्लॉक मेनू से एक गोल `repetitions`{:class="block3variables"} ब्लॉक जोड़ें:

![Nadia स्प्राइट आइकन](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
```

--- /task ---

अब, आप व्यायाम निर्देश जोड़ना शुरू कर देंगे।

--- task ---

`Text to Speech`{:class="block3extensions"} ब्लॉक मेन्यू से, एक `speak`{:class="block3extensions"} ब्लॉक जोड़ें और टेक्स्ट में टाइप करें `roll your neck to the right`।

इसके बाद,`switch costume to`{:class="block3looks"} ब्लॉक जोड़ें और उसमे `head right`{:class="block3looks"} कॉस्ट्यूम चुनें।

Finally, add a short `wait`{:class="block3control"} block:

![Nadia स्प्राइट आइकन](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
+     speak [roll your neck to the right] :: tts
+     switch costume to (head right v)
+     wait (0.5) seconds
end
```

--- /task ---

प्रत्येक व्यायाम चरण के लिए <`Text to Speech`{:class="block3extensions"}, `switch costume to`{:class="block3looks"}, और `wait`{:class="block3control"} ब्लॉक की आवश्यकता होगी।

--- task ---

निम्नलिखित `Text to Speech`{:class="block3extensions"} निर्देश जोड़ें: `and round to the left`।

ब्लॉक जोड़ें ताकि आपका **Nadia** स्प्राइट `switch costume to`{:class="block3looks"} `head left`{:class="block3looks"} करे और `0.5` सेकेंड के लिए `wait`{:class="block3control"} करे:

![Nadia स्प्राइट आइकन](images/nadia_sprite.png)

```blocks3

repeat (repetitions)
    speak [roll your neck to the right] :: tts
    switch costume to (head right v)
    wait (0.5) seconds
+     speak [and round to the left] :: tts
+     switch costume to (head left v)
+     wait (0.5) seconds
end
```

--- /task ---

अब, आप व्यायाम के अंतिम चरण को जोड़ देंगे।

--- task ---

निर्देश में टाइप करें `and back to centre`। फिर,`switch costume to`{:class="block3looks"} ब्लॉक जोड़ें और इसे <`at rest`{:class="block3looks"} पर फिर से सेट करें, फिर इसे `wait`{:class="block3control"} और `0.5` सेकंड के लिए सेट करें:

![Nadia स्प्राइट आइकन](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
    speak [roll your neck to the right] :: tts 
    switch costume to (head right v)
    wait (0.5) seconds
    speak [and round to the left] :: tts 
    switch costume to (head left v)
    wait (0.5) seconds
+     speak [and back to centre] :: tts 
+     switch costume to (at rest v)
+     wait (0.5) seconds
end
```

--- /task ---

--- task ---

अब, अपनी नई व्यायाम दिनचर्या को अपने मौजूदा कोड में जोड़ें:

--- no-print ---

![नए कोड को मौजूदा से जोड़ना](images/joinCode.gif)

--- /no-print ---

--- print-only ---

```blocks3
when flag clicked
set [repetitions v] to (3)
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
repeat (repetitions ::variables)
    switch costume to (breathe in v)
    say [breathe in]  for (2) seconds
    switch costume to (at rest v)
    say [breathe out]  for (2) seconds
end
+ repeat (repetitions)
    speak [roll your neck to the right] :: tts 
    switch costume to (head right v)
    wait (0.5) seconds
    speak [and round to the left] :: tts 
    switch costume to (head left v)
    wait (0.5) seconds
    speak [and back to centre] :: tts 
    switch costume to (at rest v)
    wait (0.5) seconds
end
```

--- /print-only ---

--- /task ---

--- save ---
