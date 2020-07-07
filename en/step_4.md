## Breathe

Let's start coding a relaxing, breathing exercise using different sprite costumes.

--- task ---

Select the **Nadia** sprite and add a `repeat`{:class="block3events"} loop to the existing code, setting the number of `repeats`{:class="block3events"} to `2`.

Inside the `repeat`{:class="block3events"} loop add a `switch costume`{:class="block3looks"} block and a `say`{:class="block3looks"} block.

Set the costume to `breathe in`{:class="block3looks"} and the `say`{:class="block3looks"} text to `breathe in`:

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

Now add another costume change with some accompaning text.

--- task ---

Select `Switch costume`{:class="block3looks"} to `at rest`{:class="block3looks"}, and type in to the `say`{:class="block3looks"} block the words `breathe out`:

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

That's the first exercise done. 

Test your script so far by clicking the green flag. 
+ Did the costume change to look like breathing? 
+ Did it repeat the routine twice?

--- save ---
