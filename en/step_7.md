## Head roll

Now you can control the number of times each exercise repeats, it is time to add a second exercise routine.

--- task ---

Select your **Nadia** sprite and select a `repeat`{:class="block3control"} block.

This exerecise should repeat the same number of times as the existing exercise so add a rounded `repetitions`{:class="block3variables"} variable block into the empty field.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
```

--- /task ---

--- task ---

For this exercise, you will use `text to speech`{:class="block3extensions"} instead of `say`{:class="block3looks"} so that the exercise instructions will be said out loud by the computer.

Click on the 'Choose an Extensions' button in the bottom left of the Scratch window.

![Extensions button](images/extensionsButton.png)

Choose the `Text to Speech`{:class="block3extensions"} extension.

![Text to speech extension](images/textToSpeechExtension.png)

A new set of `Text to Speech`{:class="block3extensions"} blocks will appear.

![Text to speech blocks](images/textToSpeechBlocks.png)

--- /task ---

Next, you're ready to start adding the exercise instructions.

--- task ---

Add a `speak`{:class="block3extensions"} block from the new `Text to Speech`{:class="block3extensions"} blocks.

Set the text to `roll your neck to the right`.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
+     speak [roll your neck to the right] :: tts
end
```

--- /task ---

--- task ---

Next, go to`Looks`{:class="block3looks"} and add a `change the costume`{:class="block3looks"} block.

Switch the costume to `head right`.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
    speak [roll your neck to the right] :: tts
+     switch costume to (head right v)
end
```

--- /task ---

You will need to add a short `wait`{:class="block3control"} block to the `text to speech`{:class="block3extensions"}. This is because it is read out more quickly than the `say`{:class="block3looks"} block (which lasts 2 seconds).

--- task ---

Add 0.5 seconds to the `wait`{:class="control"} block.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
repeat (repetitions)
    speak [roll your neck to the right] :: tts
    switch costume to (head right v)
+     wait (0.5) seconds
end
```

--- /task ---

`Text to Speech`{:class="block3extensions"}, `switch costume`{:class="block3looks"} and `wait`{:class="control"} will create each step of the exercise. Let's add the next step.

--- task ---

Add the following `Text to Speech`{:class="block3extensions"} instruction: "and around to the left".

`Switch the costume`{:class="block3looks"} to `head left` and `wait`{:class="control"} for half a second.

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

And the last step of the exercise.

--- task ---

Type in the instruction, "and back to centre" .Then add `switch the costume`{:class="block3looks"} back to `at rest` and `wait`{:class="control"} for another 0.5 seconds.

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

Now add your new exercise routine to your exisiting code.

![Nadia sprite icon](images/nadia_sprite.png)

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

--- /task ---
