## ಉಸಿರಾಟದ ವ್ಯಾಯಾಮವನ್ನು ಸೇರಿಸಿ

ಈಗ, ನೀವು ಬೇರೆ ಬೇರೆ ಸ್ಪ್ರೈಟ್‌ ಉಡುಪುಗಳನ್ನು ಉಪಯೋಗಿಸಿ ವಿಶ್ರಾಂತಿಯ ಉಸಿರಾಟದ ವ್ಯಾಯಾಮಗಳಿಗೆ ಕೋಡ್‌ ಮಾಡಲು ಪ್ರಾರಂಭಿಸುತ್ತೀರಿ.

--- task ---

**Nadia** ಸ್ಪ್ರೈಟ್‌ ಆಯ್ಕೆಮಾಡಿ ಮತ್ತು ಈಗಾಗಲೇ ಇರುವ ಕೋಡ್‌ಗೆ `repeat`{:class="block3events"} ಲೂಪ್‌ ಸೇರಿಸಿ. `repeats`{:class="block3events"} ಸಂಖ್ಯೆಗಳನ್ನು `2`ಕ್ಕೆ ಹೊಂದಿಸಿ.

`repeat`{:class="block3events"} ಲೂಪ್‌ ಒಳಗೆ, `switch costume to`{:class="block3looks"} ಬ್ಲಾಕ್‌ ಮತ್ತು `say`{:class="block3looks"} ಬ್ಲಾಕ್‌ ಸೇರಿಸಿ.

ಉಡುಪನ್ನು `breathe in`{:class="block3looks"}ಗೆ ಹೊಂದಿಸಿ ಮತ್ತು `say`{:class="block3looks"} ಪಠ್ಯವನ್ನು `breathe in` ಗೆ ಹೊಂದಿಸಿ:

![ನಾದಿಯಾ ಸ್ಪ್ರೈಟ್‌ ಐಕಾನ್](images/nadia_sprite.png)

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

`say`{:class="block3looks"} `breathe in` `for`{:class="block3looks"} `2` `seconds`{:class="block3looks"}ರಲ್ಲಿ `2` Scratchಗೆ Stage ಮೇಲೆ ಎಷ್ಟು ಸಮಯ ಮಾತಿನ ಗುಳ್ಳೆ ತೋರಿಸಬೇಕು ಎಂದು ಹೇಳುತ್ತದೆ.

ಈಗ, `repeat`{:class="block3events"} ಲೂಪ್‌ ಒಳಗೆ, ಇನ್ನೊಂದು ಉಡುಪು ಬದಲಾವಣೆಯನ್ನು ಕೆಲವು ಪಠ್ಯದೊಂದಿಗೆ ಸೇರಿಸಿ.

--- task ---

`switch costume`{:class="block3looks"}ನ್ನು `at rest`{:class="block3looks"}ಗೆ ಹೊಂದಿಸಿ, ಮತ್ತು `say`{:class="block3looks"} ಬ್ಲಾಕ್‌ನಲ್ಲಿ `breathe out` ಟೈಪ್‌ ಮಾಡಿ:

![ನಾದಿಯಾ ಸ್ಪ್ರೈಟ್‌ ಐಕಾನ್](images/nadia_sprite.png)

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

ನೀವು ಮೊದಲನೆಯ ವ್ಯಾಯಾಮವನ್ನು ಮುಗಿಸಿದ್ದೀರಿ!

ನಿಮ್ಮ ಈವರೆಗಿನ ಬರಹವನ್ನು ಪರೀಕ್ಷಿಸಲು, ಹಸಿರು ಬಾವುಟದ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ.
+ ಸ್ಪ್ರೈಟ್‌ ಉಸಿರಾಡುತ್ತಿರುವಂತೆ ಕಾಣಲು ಉಡುಪು ಬದಲಾಯಿತೇ?
+ ನಿಮ್ಮ ಪ್ರೋಗ್ರಾಮ್‌ ದಿನಚರಿಯನ್ನು ಎರಡು ಬಾರಿ ಪುನರಾವರ್ತಿಸಿತೇ?

--- save ---
