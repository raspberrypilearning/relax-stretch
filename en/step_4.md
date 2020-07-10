## Breathe

Now, you will start coding a relaxing breathing exercise using different sprite costumes.

--- task ---

Select the **Nadia** sprite and add a `repeat`{:class="block3events"} loop to the existing code. Set the number of `repeats`{:class="block3events"} to `2`.

Inside the `repeat`{:class="block3events"} loop, add a `switch costume to`{:class="block3looks"} block and a `say`{:class="block3looks"} block.

Set the costume to `breathe in`{:class="block3looks"} and set the `say`{:class="block3looks"} text to `breathe in`:

![Nadia sprite icon](images/nadia_sprite.png)

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

The `2` in `say`{:class="block3looks"} `breathe in` `for`{:class="block3looks"} `2` `seconds`{:class="block3looks"} tells Scratch how long to show the speech bubble on the Stage.

Now, within the `repeat`{:class="block3events"} loop, add another costume change with some accompanying text.

--- task ---

Set `switch costume`{:class="block3looks"} to `at rest`{:class="block3looks"}, and type `breathe out` in the `say`{:class="block3looks"} block:

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

You have finished the first exercise! 

To test your script so far, click on the green flag. 
+ Did the costume change to look like the sprite was breathing? 
+ Did your program repeat the routine twice?

--- save ---
