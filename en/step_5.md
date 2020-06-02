## The repetitions variable

Next you'll create a variable that will eventually allow the _user_ to control the number of repetitions of each exercise.

--- task ---

Go to the `Variables`{:class="block3variables"} block palette and click `Make a Variable`.

In the _dialogue box_ that opens up, give the new variable the name `repetitions`.

![Making a new variable dialogue box](images/createRepetitionsVariable.png)

The new variable will appear in the `Variables`{:class="block3variables"} palette and also in the main stage area. 

Untick the box next to `repetitions`{:class="block3variables"} in the block palette to remove the variable dsiplay box from the stage area.

![Untick the repetitions variable](images/untickRepetitionsVariable.png)

--- /task ---

The next step is to _initialise_ the new `repetitions`{:class="block3variables"} variable to give it an initial value when the program starts.

--- task ---

Make sure that your **Nadia** sprite is selected and from the `Variables`{:class="block3variables"} palette, add a `set repetitions to`{:class="block3variables"} block and set the variable to 3.

```blocks3
+ set [repetitions v] to (3)
when flag clicked
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

