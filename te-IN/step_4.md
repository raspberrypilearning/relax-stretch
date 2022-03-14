## Repetitions ని నియంత్రించండి

ఇప్పుడు, మీరు ప్రతి వ్యాయామం యొక్క repetitions సంఖ్యను నియంత్రించడానికి యూజర్ ని అనుమతించే వేరియబుల్‌ను సృష్టిస్తారు.

--- task ---

`Variables`{:class="block3variables"} బ్లాక్స్ మెనుకి వెళ్లి, **Make a Variable**పై క్లిక్ చేసి, దానికి `repetitions` అని పేరు పెట్టండి.

![కొత్త వేరియబుల్ డైలాగ్ బాక్స్‌ను తయారు చేయడం](images/createRepetitionsVariable.png){:width=“200px”}

కొత్త వేరియబుల్ ఇప్పుడు `Variables`{:class="block3variables"} బ్లాక్స్ మెనులో మరియు Stageలో కూడా కనిపిస్తుంది.

--- /task ---

ప్రోగ్రామ్ మొదలయిన తరువాత `repetitions`{:class="block3variables"} విలువను సెట్ చేయడం తదుపరి దశ.

--- task ---

**Nadia** sprite సెలెక్ట్ చేసిన తరువాత, `set repetitions to`{:class="block3variables"} బ్లాక్‌ ని జోడించి, విలువను `3` గా సెట్ చేయండి:

![Nadia sprite చిహ్నం](images/nadia_sprite.png)

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

ఇప్పుడు, మీరు వ్యాయామం పునరావృతమయ్యే సంఖ్యను నియంత్రించడానికి `repetitions`{:class="block3variables"} ని ఉపయోగించవచ్చు.

--- task ---

`repeat`{:class="block3control"} బ్లాక్ యొక్క విలువగా ఒక రౌండెడ్ `repetitions`{:class="block3variables"} బ్లాక్‌ను జోడించండి:

![Nadia sprite చిహ్నం](images/nadia_sprite.png)

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

ఈ ప్రోగ్రామ్ పని చేస్తుందో లేదో తనిఖీ చేయడానికి `repetitions`{:class="block3variables"} విలువను మార్చవచ్చు మరియు ప్రోగ్రామ్‌ను అమలు చేయవచ్చు.

--- save ---
