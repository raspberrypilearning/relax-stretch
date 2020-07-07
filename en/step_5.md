## Repetitions

Next, you'll create a variable that will eventually allow a user to control the number of repetitions of each exercise.

--- task ---

Go to the `Variables`{:class="block3variables"} block, click `Make a Variable` and name it `repetitions`.

![Making a new variable dialogue box](images/createRepetitionsVariable.png)

The new variable will now appear in the `Variables`{:class="block3variables"} blocks section and also in the Stage. 

--- /task ---

The next step is to set the value of `repetitions`{:class="block3variables"} when the program starts.

--- task ---

With the **Nadia** sprite selected, add a `set repetitions to`{:class="block3variables"} block and set the value to `3`:

![Nadia sprite icon](images/nadia_sprite.png)

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

Now let's use `repetitions`{:class="block3variables"} to control the number of times the exercise repeats. 

--- task ---

Add a rounded `repetitions`{:class="block3variables"} block as the value of the `repeat`{:class="block3control"} block:

![Nadia sprite icon](images/nadia_sprite.png)

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

--- /task ---

One way to check that this program works is by changing the value of `repetitions`{:class="block3variables"} and running the program.

--- save ---
