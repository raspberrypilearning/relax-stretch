## ಬಟನ್‌ಗಳನ್ನು ಕೋಡ್‌ ಮಾಡಿ

ಈಗ, ನೀವು ಬಟನ್‌ಗಳನ್ನು ಕ್ಲಿಕ್‌ ಮಾಡಿದಾಗ `repetitions`{:class="block3variables"} ಮೌಲ್ಯವನ್ನು ಬದಲಾಯಿಸಲು ಬಾಣದ ಬಟನ್‌ಗಳನ್ನು ಕೋಡ್‌ ಮಾಡುತ್ತೀರಿ.

--- task ---

**up** ಸ್ಪ್ರೈಟ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ. ಅಸ್ತಿತ್ವದಲ್ಲಿರುವ ಕೋಡ್‌ನ್ನು ಹಾಗೆಯೇ ಬಿಡಿ. `when this sprite clicked`{:class="block3events"} ಬ್ಲಾಕ್‌ನ್ನು ಆಯ್ಕೆ ಮಾಡಿ.

`change repetitions by`{:class="block3variables"} ಬ್ಲಾಕ್‌ನ್ನು ಈ ಕೆಳಗಿನ `Variables`{:class="block3variables"} ಬ್ಲಾಕ್‌ಗಳ ಮೆನುನಿಂದ ಸೇರಿಸಿ. ಇದರ ಮೌಲ್ಯ `1` ಆಗಿರಬೇಕು:

![ಅಪ್‌ ಬಾಣ ಸ್ಪ್ರೈಟ್‌ನ ಐಕಾನ್](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
change [repetitions v] by (1)
```

--- /ಕಾರ್ಯ ---

ಹಸಿರು ಬಾವುಟದ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು ಪ್ರತಿಯೊಂದು ಬಾರಿ **up** ಬಾಣದ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿದಾಗ `repetitions`{:class="block3variables"} ಮೇಲಕ್ಕೇರುತ್ತದೆಯೇ ಎಂದು ಪರೀಕ್ಷಿಸಿ.

ಮುಂದುವರಿಸಿ. `repetitions`{:class="block3variables"} ಮೇಲಕ್ಕೇರುವುದನ್ನು ನಿಲ್ಲಿಸುತ್ತದೆಯೇ?

ನಿಮಗೆ ವ್ಯಾಯಾಮವು ಬಹಳಷ್ಟು ಸಮಯ ಪುನರಾವರ್ತನೆಯಾಗಬಾರದು, ಆದುದರಿಂದ ನಂತರ, ನೀವು `repetitions`{:class="block3variables"} 5ಕ್ಕಿಂತ ಮೇಲಕ್ಕೇರುವುದನ್ನು ನಿಲ್ಲಿಸಲು ಯಾವುದಾದರೂ ಕೋಡ್‌ ಸೇರಿಸುತ್ತೀರಿ.

--- task ---

`Control`{:class="block3control"} ಬ್ಲಾಕ್‌ಗಳ ಮೆನುನಿಂದ, `if ... then ... else`{:class="block3control"} ಬ್ಲಾಕ್‌ನ್ನು ಆಯ್ಕೆ ಮಾಡಿ, ಮತ್ತು `change repetitions by 1`{:class="block3variables"} ಬ್ಲಾಕ್‌ನ್ನು `if ... then`{:class="block3control"}ರ ಕೆಳಗಿನ ಖಾಲಿ ಜಾಗದಲ್ಲಿ ಇಡಿ:

![ಅಪ್‌ ಬಾಣ ಸ್ಪ್ರೈಟ್‌ನ ಐಕಾನ್](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
+ if <> then
    change [repetitions v] by (1)
else
+ end
```

--- /task ---

ಈಗ, ನೀವು `if`{:class="block3control"} `repetitions`{:class="block3variables"} `is less than`{:class="block3operators"} `5` ಷರತ್ತನ್ನು ಸೇರಿಸುತ್ತೀರಿ.

**ಸೂಚನೆ:** ಇದು ಪುನರಾವರ್ತನೆಯ ಗರಿಷ್ಢ ಸಂಖ್ಯೆಯನ್ನು ಹೊಂದಿಸುತ್ತದೆ. ನೀವು ಬೇರೆ ಸಂಖ್ಯೆಯನ್ನು ಆಯ್ಕೆ ಮಾಡಿಕೊಳ್ಳಬಹುದು ಆದರೆ ನೀವು ಹೆಚ್ಚು ಪುನರಾವರ್ತನೆಗಳಿಗೆ ಅನುವುಮಾಡಿಕೊಟ್ಟರೆ, ಪ್ರೋಗ್ರಾಮ್‌ ರನ್‌ ಆಗಲು ಹೆಚ್ಚು ಸಮಯ ತೆಗದುಕೊಳ್ಳುತ್ತದೆ.

--- task ---

`Operators`{:class="block3operators"} ಬ್ಲಾಕ್‌ಗಳ ಮೆನುನಿಂದ, `less than`{:class="block3operators"} ಆಪರೇಟರ್‌ ಆಯ್ಕೆಮಾಡಿಕೊಳ್ಳಿ:

```blocks3
[]<[] ::operators
```

`if`{:class="block3control"} ಮತ್ತು `then`{:class="block3control"} ಗಳ ನಡುವೆ.`if ... then ... else`{:class="block3control"} ಬ್ಲಾಕ್‌ನ ಮೇಲಿನ ಖಾಲಿ ಜಾಗದಲ್ಲಿ ಇಡಿ.

`Variables`{:class="block3variables"} ಬ್ಲಾಕ್‌ಗಳ ಮೆನುನಿಂದ, ಪೂರ್ಣಾಂಕ `repetitions`{:class="block3variables"} ಬ್ಲಾಕ್‌ನ್ನು ತೆಗದುಕೊಳ್ಳಿ ಮತ್ತು ಅದನ್ನು `<`{:class="block3operators"}ಕ್ಕಿಂತ ಮೊದಲು ಇಡಿ. `5` ಸಂಖ್ಯೆಯನ್ನು `<`{:class="block3operators"} ನಂತರ ಟೈಪ್‌ ಮಾಡಿ:

![ಅಪ್‌ ಬಾಣ ಸ್ಪ್ರೈಟ್‌ನ ಐಕಾನ್](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators +> then
    change [repetitions v] by (1)
else
end
```

--- /ಕಾರ್ಯ ---

ಈಗ, `repetitions`{:class="block3variables"} `1` `if`{:class="block3control"} `repetitions`{:class="block3variables"} `is less than`{:class="block3operators"} `5`ಕ್ಕಿಂತ ಕಡಿಮೆ ಇದ್ದಾಗ ಮಾತ್ರ ಮೇಲಕ್ಕೇರಬೇಕು.

ಬಳಕೆದಾರ `repetitions`{:class="block3variables"}ನ್ನು 5 ಅಥವಾ ಅದಕ್ಕಿಂತ ಹೆಚ್ಚಿನದಕ್ಕೆ ಹೊಂದಿಸಿದರೆ ಏನಾಗುತ್ತದೆ?

--- task ---

`else`{:class="block3control"}ರ ಕೆಳಗೆ, ಗರಿಷ್ಠ `5 ಪುನರಾವರ್ತನೆಗಳು ಎಂದು <code>2` ಸೆಕೆಂಡುಗಳ </code> ವರೆಗೆ ಸಂದೇಶ ತೋರಿಸುವ `say`{:class="block3looks"} ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ:

![ಅಪ್‌ ಬಾಣ ಸ್ಪ್ರೈಟ್‌ನ ಐಕಾನ್](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators> then
    change [repetitions v] by (1)
else
+     say [5 repetitions is the maximum] for (2) seconds
end
```

--- /task ---

ಈಗ, ನೀವು **down** ಬಾಣಕ್ಕೂ ಸಹ ಅದನ್ನೆ ಮಾಡಬೇಕು, ಆದರೆ ನೀವು ಬೇರೆ ಷರತ್ತನ್ನು ಉಪಯೋಗಿಸಬೇಕು ಮತ್ತು `repetitions`{:class="block3variables"}ನ್ನು ಪ್ರತಿಬಾರಿ 1 ರಷ್ಟು ಕಡಿಮೆಮಾಡಬೇಕು.

Scratch ನಲ್ಲಿ **reduce by 1** ಎಂದು ಹೇಳುವ ವಿಧಾನ ಎಂದರೆ `change by`{:class="block3variables"} `-1`.

--- task ---

**down** ಸ್ಪ್ರೈಟ್‌ ಆಯ್ಕೆ ಮಾಡಿಕೊಳ್ಳಿ. `when this sprite clicked`{:class="block3events"} ಬ್ಲಾಕ್‌ನ್ನು ಮತ್ತು `if ... then ... else`{:class="block3control"} ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ.

`if`{:class="block3control"} `repetitions`{:class="block3variables"} `is more than`{:class="block3operators"} `1` ಷರತ್ತನ್ನು ಸೇರಿಸಿ.

ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ, ಅದರಿಂದ ಷರತ್ತು **true** ಆದರೆ, ನಿಮ್ಮ ಪ್ರೋಗ್ರಾಮ್‌ `change repetitions by`{:class="block3variables"} `-1` ಮಾಡುತ್ತದೆ.

ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ, ಅದರಿಂದ ಷರತ್ತು **false** ಆದರೆ, ನಿಮ್ಮ ಪ್ರೋಗ್ರಾಮ್‌ `say`{:class="block3looks"} `Repetitions can't be lower than 1` ಎಂದು `2` ಸೆಕೆಂಡುಗಳ ಕಾಲ ಹೇಳುತ್ತದೆ:

![ಡೌನ್ ಬಾಣ ಸ್ಪ್ರೈಟ್‌ನ ಐಕಾನ್](images/down_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions)>[1]> then
    change [repetitions v] by (-1)
else
    say [Repetitions can't be lower than 1] for (2) seconds
end
```

--- /task ---

ಅದನ್ನು ಪರೀಕ್ಷಿಸಲು ಪ್ರಾಜೆಕ್ಟ್‌ನ್ನು ರನ್ ಮಾಡಿ. ಪುನರಾವರ್ತನೆಗಳ ಸಂಖ್ಯೆಯನ್ನು ಹೆಚ್ಚಿಸಲು ಅಥವಾ ಕಡಿಮೆ ಮಾಡಲು ಎರಡು ಬಾಣಗಳ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ.

`repetitions`{:class="block3variables"} 1 ಮತ್ತು 5ರ ನಡುವೆ ಇರುತ್ತದೆಯೇ?

--- save ---
