## శ్వాస కోశ వ్యాయామాన్ని జోడించండి

ఇప్పుడు, మీరు వివిధ sprite costume లను ఉపయోగించి రిలాక్సింగ్ శ్వాస వ్యాయామాన్ని కోడ్ చేయడం ప్రారంభిస్తారు.

--- task ---

**Nadia** sprite ని సెలెక్ట్ చేసి `repeat`{:class="block3events"} లూప్‌ని కోడ్ కి జోడించండి. `repeats`{:class="block3events"} సంఖ్యని `2` కు సెట్ చేయండి.

`repeat`{:class="block3events"} లూప్ లోపల,`switch costume`{:class="block3looks"} బ్లాక్‌కి మరియు `say`{:class="block3looks"} బ్లాక్‌ని జోడించండి.

Costume ని `breathe in`{:class="block3looks"} కి సెట్ చేయండి మరియు `say`{:class="block3looks"} టెక్స్ట్‌ని `breathe in` కి సెట్ చేయండి:

![Nadia sprite చిహ్నం](images/nadia_sprite.png)

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

`say`{:class="block3looks"} లో `2` `breath in` `for`{:class="block3looks"} `2` `seconds`{:class="block3looks"} Scratch కి ఎంత సమయం Stage పై స్పీచ్ బబుల్ ను చూపించాలో చెబుతుంది.

ఇప్పుడు, `repeat`{:class="block3events"} లూప్‌లో, కొంత వచనంతో మరొక costume మార్పును జోడించండి.

--- task ---

`switch costume`{:class="block3looks"}ని `at rest`{:class="block3looks"} కి మార్చండి, మరియు `say`{:class="block3looks"} బ్లాక్‌లో `breathe out` అని టైపు చేయండి:

![Nadia sprite చిహ్నం](images/nadia_sprite.png)

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

మీరు మొదటి వ్యాయామాన్ని పూర్తి చేసారు!

ఇప్పటివరకు మీ స్క్రిప్ట్‌ను పరీక్షించడానికి, ఆకుపచ్చ జెండాపై క్లిక్ చేయండి.
+ Sprite ఊపిరి పీల్చుకుంటున్నట్టు కనిపించేలా costume మారిందా?
+ మీ ప్రోగ్రామ్ రొటీన్‌ను రెండుసార్లు పునరావృతం చేసిందా?

--- save ---
