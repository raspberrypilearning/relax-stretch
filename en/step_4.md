## Exercise 1

It is time to start coding a relaxing, breathing exercise using different sprite costumes.

--- task ---

Select the **Nadia** sprite and add a `repeat`{:class="block3events"} loop to the existing code.

For now, set the number of `repeats`{:class="block3events"} to `2`.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
+ repeat (2)
end
```

--- /task ---

--- task ---

From `Looks`{:class="block3looks"}, add a `switch the costume`{:class="block3looks"} block inside the `repeat`{:class="block3events"} block.

Select the costume `breathe in`{:class="block3looks"}.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
repeat (2)
+     switch costume to (breathe in v)
end
```

--- /task ---

Now add an instruction to go with the costume change. Here, you will use a `say`{:class="block3looks"} block to display a speech bubble. Later you will use `text to speech`{:class="block3extensions"}.

--- task ---

From `Looks`{:class="block3looks"}, select a `say`{:class="block3looks"} block and type in the text "breathe in". Add it below the `switch the costume`{:class="block3looks"} block.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
repeat (2)
    switch costume to (breathe in v)
+     say [breathe in]  for (2) seconds
end
```

--- /task ---

Now add another costume change along with its instruction.

--- task ---

Add a `switch costume to`{:class="block3looks"} block and set the new costume to `at rest`.

Under that, add another `say`{:class="block3looks"} block and type in the text "breathe out".

![Nadia sprite icon](images/nadia_sprite.png)

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

That's the first exercise done. Try clicking the green flag and check that everything works as you expected it to.
