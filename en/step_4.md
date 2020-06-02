## Exercise 1

Time to start coding a relaxing, breathing exercise using different sprite costumes.

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

Inside the `repeat`{:class="block3events"} loop, add a `Looks`{:class="block3looks"} block to `switch the costume`{:class="block3looks"}.

Set the costume to `breathe in`{:class="block3looks"}.

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