## Head roll

Now that you can control the number of times that each exercise repeats, it is time to add a second exercise routine.

--- task ---

For this exercise, you will use `Text to Speech`{:class="block3extensions"} instead of `say`{:class="block3looks"} so that the exercise instructions will be spoken by the computer.

Click the **Add Extension** button in the bottom left-hand corner of the Scratch window.

![Extensions button](images/extensionsButton.png)

Select the `Text to Speech`{:class="block3extensions"} extension.

![Text to Speech extension](images/textToSpeechExtension.png)

A new set of `Text to Speech`{:class="block3extensions"} blocks will appear.

![Text to Speech blocks](images/textToSpeechBlocks.png)

--- /task ---

Next, you will create the head roll exercise as a separate block of code, which you will add to your main code at the end.

--- task ---

Choose the **Nadia** sprite and select a `repeat`{:class="block3control"} block.

Add a rounded `repetitions`{:class="block3variables"} variable block to control the number of repetitions:

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
```

--- /task ---

Now, you will start adding the exercise instructions.

--- task ---

From the `Text to Speech`{:class="block3extensions"} menu, add a `speak`{:class="block3extensions"} block and type in the text `roll your neck to the right`.

Next, add a `switch costume to`{:class="block3looks"} block and select the costume `head right`.

Lastly, add a short `wait`{:class="block3control"} block: 

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
+     speak [roll your neck to the right] :: tts
+     switch costume to (head right v)
+     wait (0.5) seconds
end
```

--- /task ---

Each exercise step will use `Text to Speech`{:class="block3extensions"}, `switch costume to`{:class="block3looks"}, and `wait`{:class="control"} blocks.

--- task ---

Add the following `Text to Speech`{:class="block3extensions"} instruction: `and around to the left`.

`switch costume to`{:class="block3looks"} `head left`{:class="block3looks"} and `wait`{:class="control"} for 0.5 seconds:

![Nadia sprite icon](images/nadia_sprite.png)

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

Now, you will add the last step of the exercise.

--- task ---

Type in the instruction `and back to centre`. Then, add `switch costume to`{:class="block3looks"} and set it back to `at rest`, and `wait`{:class="control"} for another 0.5 seconds:

![Nadia sprite icon](images/nadia_sprite.png)

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

Now, add your new exercise routine to your existing code:

--- no-print ---

![Joining new code to existing](images/joinCode.gif)

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
