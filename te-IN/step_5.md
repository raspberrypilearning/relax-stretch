## బటన్లను కోడ్ చేయండి

బటన్లు క్లిక్ చేసినపుడు `repetitions`{:class="block3variables"} విలువను మార్చడానికి బాణం గుర్తుల బటన్‌లను ఇప్పుడు మీరు కోడ్ చేస్తారు.

--- task ---

**up** sprite పై క్లిక్ చేయండి. ఇప్పటికే ఉన్న కోడ్‌ని అలాగే వదిలేయండి. `when this sprite clicked`{:class="block3events"} బ్లాక్‌ని ఎంచుకోండి.

`Variables`{:class="block3variables"} బ్లాక్‌ల మెను నుంచి, `change repetitions by`{:class="block3variables"} బ్లాక్ ని జోడించండి. దీని విలువ `1` ఉండాలి:

![Up బాణం sprite చిహ్నం](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
change [repetitions v] by (1)
```

--- /task ---

ఆకుపచ్చ జెండాపై క్లిక్ చేసి, **up** బాణంపై క్లిక్ చేసినప్పుడల్లా `repetitions`{:class="block3variables"} విలువ పెరుగుతుందో, లేదో పరీక్షించండి.

ముందుకు వెళ్తూ ఉండండి. `repetitions`{:class="block3variables"} పెరగడం ఆగి పోయిందా?

మీరు వ్యాయామం చాలాసార్లు పునరావృతం చేయకూడదనుకుంటున్నారు, కాబట్టి తర్వాత, మీరు `repetitions`{:class="block3variables"} ని 5 కంటే పైకి వెళ్లకుండా ఆపడానికి కొంత కోడ్‌ని జోడిస్తారు.

--- task ---

`Control`{:class="block3control"} బ్లాక్‌ల మెను నుండి, `if ... then ... else`{:class="block3control"} బ్లాక్‌ని ఎంచుకోండి మరియు `change repetitions by 1` {: class="block3variables"} ని, `if ... then`{:class="block3control"}: బ్లాక్ కింద ఉన్న స్పేస్‌లో ఉంచండి

![Up బాణం sprite చిహ్నం](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
+ if <> then
    change [repetitions v] by (1)
else
+ end
```

--- /task ---

ఇప్పుడు,`if`{:class="block3control"} `repetitions`{:class="block3variables"} `is less than`{:class="block3operators"} `5` కండిషన్ ను జోడిస్తారు.

**గమనిక:** ఇది పునరావృతాల గరిష్ట సంఖ్యను సెట్ చేస్తుంది. మీరు వేరొక సంఖ్యను ఎంచుకోవచ్చు కానీ మీరు ఎక్కువ పునరావృతాలను అనుమతించినట్లయితే, ప్రోగ్రామ్ రన్ చేయడానికి ఎక్కువ సమయం పడుతుంది.

--- task ---

`Operators`{:class="block3operators"} బ్లాక్స్ మెను నుండి,</code>less than`{:class="block3operators"} ఆపరేటర్‌ని ఎంచుకోండి:</p>

<pre><code class="blocks3">[]<[] ::operators
`</pre>

బ్లాక్‌ను `if ... then ... else`{:class="block3control"} బ్లాక్ లో పైన ఉన్న ఖాళీలో, `if`{:class="block3control"} మరియు `then`{:class= "block3control"} మధ్యలో ఉంచండి.

`Variables`{:class="block3variables"} బ్లాక్‌ల మెను నుండి, రౌండెడ్ `repetitions`{:class="block3variables"} బ్లాక్‌ని తీసుకుని, దానిని `<`{:class="block3operators"} ముందు ఉంచండి. `<`{:class="block3operators"} తర్వాత `5` సంఖ్యను టైప్ చేయండి:

![Up బాణం sprite చిహ్నం](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators +> then
    change [repetitions v] by (1)
else
end
```

--- /task ---

`if`{:class="block3control"} `repetitions`{:class="block3variables"} `5`.`is less than 1` {: class="block3operators"} ఇప్పుడు, `repetitions`{:class="block3variables"} `1` గా మాత్రమే పెరగాలి.

`repetitions`{:class="block3variables"} విలువని 5 లేదా అంతకంటే ఎక్కువకు సెట్ చేస్తే ఏమి జరుగుతుంది?

--- task ---

`else`{:class="block3control"} క్రింద, `say`{:class="block3looks"} బ్లాక్‌ను జోడించండి, అది `5 repetitions the maximum` `2` సెకండ్లకు అనే సందేశాన్ని ప్రదర్శిస్తుంది:

![Up బాణం sprite చిహ్నం](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators> then
    change [repetitions v] by (1)
else
+     say [5 repetitions is the maximum] for (2) seconds
end
```

--- /task ---

**down** బాణం గుర్తు కోసం అదే విధంగా చేయాలి, కానీ మీరు వేరొక కండిషన్ ను ఉపయోగించి `repetitions`{:class="block3variables"} ను 1కి తగ్గించాలి.

Scratch లో **reduce by 1 ** చెప్పడానికి ఒక మార్గం `change by`{:class="block3variables"} `-1`.

--- task ---

**down** sprite ని ఎంచుకోండి. `when this sprite clicked `{:class="block3events"} బ్లాక్‌ని మరియు `if ... then ...else`{:class="block3control"} బ్లాక్‌ని జోడించండి.

`if`{:class="block3control"} `repetitions`{:class="block3variables"} `is more than`{:class="block3operators"} `1` కండిషన్ ను జోడించండి.

కండిషన్ **true** అయితే, మీ ప్రోగ్రామ్ `change repetitions by`{:class="block3variables"} `-1` గా మార్చేలా బ్లాక్ ను జోడించండి.

కండిషన్ **false** అయితే, మీ ప్రోగ్రామ్ `Repetitions can't be lower than 1` ప్రతి `2` సెకండ్స్ కి అని చెప్పేలా `say `{:class="block3looks"} బ్లాక్‌ని జోడించండి:

![Down బాణం sprite చిహ్నం](images/down_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions)>[1]> then
    change [repetitions v] by (-1)
else
    say [Repetitions can't be lower than 1] for (2) seconds
end
```

--- /task ---

దీన్ని పరీక్షించడానికి ప్రోగ్రామ్‌ను అమలు చేయండి. repetitions సంఖ్యను పెంచడానికి లేదా తగ్గించడానికి రెండు బాణపు గుర్తులపై క్లిక్ చేయండి.

`repetitions`{:class="block3variables"} 1 మరియు 5 మధ్య ఉంటాయా?

--- save ---
