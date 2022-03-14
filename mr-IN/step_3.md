## श्वासोच्छवासाचा व्यायाम जोडा

आता, तुम्ही वेगवेगळ्या स्प्राईट कॉश्चुमचा वापर करून आरामदायी श्वासोच्छवासाचा व्यायाम कोड करणे चालू कराल.

--- task ---

**Nadia** sprite निवडा आणि आधीच्या कोडला `repeat`{:class="block3events"} लूप जोडा. `repeats`{:class="block3events"} ची संख्या `2` ला सेट करा.

`repeat`{:class="block3events"} लूपमध्ये, `switch costume to`{:class="block3looks"} ब्लॉक आणि `say`{:class="block3looks"} ब्लॉक जोडा.

कॉश्चुम `breathe in`{:class="block3looks"} ला सेट करा आणि `say`{:class="block3looks"} टेक्स्ट `breathe in` ला सेट करा:

![Nadia sprite आयकॉन](images/nadia_sprite.png)

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

`2` मध्ये `say`{:class="block3looks"} `breathe in` `for`{:class="block3looks"} `2` `seconds`{:class="block3looks"} हा Scratch ला Stage वर किती काळ स्पीच दाखवायची हे सांगतो.

आता, `repeat`{:class="block3events"} लूपमध्ये, काही सोबतच्या टेक्स्टसह दुसरा कॉश्चुम चेंज जोडा.

--- task ---

`switch costume`{:class="block3looks"} हा `at rest`{:class="block3looks"} ला सेट करा, आणि `breathe out` हा `say`{:class="block3looks"} ब्लॉकमध्ये टाईप करा:

![Nadia sprite आयकॉन](images/nadia_sprite.png)

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

तुम्ही पहिला व्यायाम पूर्ण केला आहे!

आतापर्यंतची तुमची स्क्रिप्ट तपासण्यासाठी, हिरव्या झेंड्यावर क्लिक करा.
+ स्प्राईट श्वास घेतल्यासारखे दिसण्यासाठी कॉश्चुम चेंज केला का?
+ तुमच्या प्रोग्रामने रूटीन दोनदा रिपीट केले का?

--- save ---
