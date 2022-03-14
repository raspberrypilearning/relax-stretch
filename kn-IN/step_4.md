## ಪುನರಾವರ್ತನೆಗಳನ್ನು ನಿಯಂತ್ರಿಸಿ

ಈಗ, ಪ್ರತಿಯೊಂದು ವ್ಯಾಯಾಮದ ಪುನರಾವರ್ತನೆಯ ಸಂಖ್ಯೆಗಳನ್ನು ಬಳಕೆದಾರ ನಿಯಂತ್ರಿಸಲು ಅಂತಿಮವಾಗಿ ಅನುವುಮಾಡಿಕೊಡುವ ವೇರಿಯೇಬಲ್‌ನ್ನು ನೀವು ರಚಿಸುತ್ತೀರಿ.

--- task ---

`Variables`{:class="block3variables"} ಬ್ಲಾಕ್‌ ಮೆನುಗೆ ಹೋಗಿ **Make a Variable** ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ, ಮತ್ತು ಅದನ್ನು `repetitions` ಎಂದು ಹೆಸರಿಸಿ.

![ಹೊಸ ವೇರಿಯೇಬಲ್‌ ಡೈಲಾಗ್‌ ಬಾಕ್ಸ್‌ ಮಾಡುವುದು](images/createRepetitionsVariable.png){:width=“200px”}

ಹೊಸ ವೇರಿಯೇಬಲ್‌ ಈಗ `Variables`{:class="block3variables"} ಬ್ಲಾಕ್‌ಗಳ ಮೆನುನಲ್ಲಿ ಮತ್ತು Stage ಮೇಲೂ ಸಹ ಕಾಣಿಸಿಕೊಳ್ಳುತ್ತದೆ.

--- /ಕಾರ್ಯ ---

ಮುಂದಿನ ಹಂತವೆಂದರೆ ಪ್ರೋಗ್ರಾಮ್‌ ಶುರುವಾದಾಗ `repetitions`{:class="block3variables"}ನ ಮೌಲ್ಯವನ್ನು ಹೊಂದಿಸುವುದು.

--- task ---

**Nadia** ಸ್ಪ್ರೈಟ್‌ ಆಯ್ಕೆಯಾಗಿರುವವಾಗ, `set repetitions to`{:class="block3variables"} ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ ಮತ್ತು ಮೌಲ್ಯವನ್ನು `3`ಕ್ಕೆ ಹೊಂದಿಸಿ:

![Nadia ಸ್ಪ್ರೈಟ್‌ ಐಕಾನ್](images/nadia_sprite.png)

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

ಈಗ, ನೀವು ಆ ವ್ಯಾಯಾಮವು ಪುನರಾವರ್ತನೆಯಾಗುವ ಸಂಖ್ಯೆಗಳನ್ನು ನಿಯಂತ್ರಿಸಲು `repetitions`{:class="block3variables"} ಉಪಯೋಗಿಸುತ್ತೀರಿ.

--- task ---

`repeat`{:class="block3control"} ಬ್ಲಾಕ್‌ನ ಮೌಲ್ಯವಾಗಿ ಪೂರ್ಣಾಂಕ `repetitions`{:class="block3variables"} ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ:

![Nadia ಸ್ಪ್ರೈಟ್‌ ಐಕಾನ್](images/nadia_sprite.png)

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

--- /ಕಾರ್ಯ ---

ಈ ಪ್ರೋಗ್ರಾಮ್‌ ಕೆಲಸಮಾಡುತ್ತದೆಯೇ ಎಂದು ಪರಿಶೀಲಿಸಲು, ನೀವು `repetitions`{:class="block3variables"}ನ ಮೌಲ್ಯವನ್ನು ಬದಲಾಯಿಸಿ ರನ್‌ ಮಾಡಬಹುದು.

--- save ---
