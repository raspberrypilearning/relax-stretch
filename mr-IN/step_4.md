## पुनरावृत्ती नियंत्रित करा

आता, तुम्ही एक व्हेरिएबल तयार कराल जे शेवटी यूजरला प्रत्येक व्यायामाच्या पुनरावृत्तीची संख्या नियंत्रित करण्यास अनुमती देईल.

--- task ---

`Variables`{:class="block3variables"} ब्लॉक मेनूवर जा, **Make a Variable** वर क्लिक करा,आणि त्याला `repetitions` असे नाव द्या.

![नवीन व्हेरिएबल डायलॉग बॉक्स बनवत आहे](images/createRepetitionsVariable.png){:width=“200px”}

नवीन व्हेरिएबल आता `Variables`{:class="block3variables"} ब्लॉक्स मेनूमध्ये आणि Stage वर सुद्धा दिसतील.

--- /task ---

प्रोग्राम चालू झाल्यावर `repetitions`{:class="block3variables"} ची व्हॅल्यू सेट करणे हा पुढचा टप्पा आहे.

--- task ---

**Nadia** sprite निवडून, `set repetitions to`{:class="block3variables"} ब्लॉक जोडा आणि व्हॅल्यू `3` ला सेट करा:

![Nadia sprite आयकॉन](images/nadia_sprite.png)

```blocks3
when flag clicked
+ set [repetitions v] to (3)
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
repeat (2)
    switch costume to (breathe in v)
    say [breathe in]  for (2) seconds
    switch costume to (at rest v)
    say [breathe out]  for (2) seconds
end
```

--- /task ---

आता, तुम्ही व्यायाम कितीवेळा रिपीट व्हावा ती संख्या नियंत्रीत करण्यासाठी `repetitions`{:class="block3variables"} वापराल.

--- task ---

`repeat`{:class="block3control"} ब्लॉकची व्हॅल्यू म्हणून गोलाकार `repetitions`{:class="block3variables"} ब्लॉक जोडा:

![Nadia sprite आयकॉन](images/nadia_sprite.png)

```blocks3
when flag clicked
set [repetitions v] to (3)
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
repeat (repetitions ::variables +)
    switch costume to (breathe in v)
    say [breathe in]  for (2) seconds
    switch costume to (at rest v)
    say [breathe out]  for (2) seconds
end
```

--- /task ---

हा प्रोग्राम कार्य करतो का हे तपासण्यासाठी, तुम्ही `repetitions`{:class="block3variables"} ची व्हॅल्यू बदलू शकता आणि प्रोग्राम रन करू शकता.

--- save ---
