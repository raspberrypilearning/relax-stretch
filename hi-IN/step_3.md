## श्वसन व्यायाम जोड़ें

अब, आप विभिन्न स्प्राइट परिधानों का उपयोग करके आराम से श्वसन व्यायाम को कोड करना शुरू करेंगे।

--- task ---

**Nadia** स्प्राइट का चयन करें और मौजूदा कोड में एक `repeat`{:class="block3events"} लूप जोड़ें। `repeats`{:class="block3events"} की संख्या को `2` पर सेट करें।

`repeat`{:class="block3events"} लूप के अंदर, एक`switch costume to`{:class="block3looks"} ब्लॉक और `say`{:class="block3looks"} ब्लॉक जोड़ें।

पोशाक को `breathe in`{:class="block3looks"} पर सेट करें और `say`{:class="block3looks"} टेक्स्ट को `breathe in`:

![Nadia स्प्राइट आइकन](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
+ repeat (2)
    switch costume to (breathe in v)
    say [breathe in]  for (2) seconds
+ end
```

--- /task ---

`2` में `say`{:class="block3looks"} `breathe in` `for`{:class="block3looks"} `2` `seconds`{:class="block3looks"} Scratch को बताता है कि कितनी देर तक Stage पर स्पीच बबल दिखाना है।

अब, `repeat`{:class="block3events"} लूप के भीतर, कुछ साथ वाले टेक्स्ट के साथ एक और कॉस्ट्यूम चेंज जोड़ें।

--- task ---

`switch costume`{:class="block3looks"} को `at rest`{:class="block3looks"} पर सेट करें, और `say`{:class="block3looks"} block: में `breathe out` टाइप करें

![Nadia स्प्राइट आइकन](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
repeat (2)
    switch costume to (breathe in v)
    say [breathe in]  for (2) seconds
+     switch costume to (at rest v)
+     say [breathe out]  for (2) seconds
end
```

--- /task ---

आपने पहला व्यायाम समाप्त कर लिया है!

अपनी अब तक की स्क्रिप्ट का परीक्षण करने के लिए, हरे झंडे पर क्लिक करें।
+ क्या कॉस्ट्यूम स्प्राइट सांस ले रहा की तरह दिखने के लिए बदला
+ क्या आपके प्रोग्राम ने दिनचर्या को दो बार दोहराया?

--- save ---
