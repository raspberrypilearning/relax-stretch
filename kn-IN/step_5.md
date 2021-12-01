## Code the buttons

Now, you will code the arrow buttons to change the value of `repetitions`{:class="block3variables"} when the buttons are clicked.

--- task ---

Click on the **up** sprite. Leave the existing code as it is. Select a `when this sprite clicked`{:class="block3events"} block.

Add a `change repetitions by`{:class="block3variables"} block from the `Variables`{:class="block3variables"} blocks menu below. This should have a value of `1`:

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
change [repetitions v] by (1)
```

--- /task ---

Click on the green flag and test that `repetitions`{:class="block3variables"} goes up each time you click on the **up** arrow.

Keep going. Does `repetitions`{:class="block3variables"} stop going up?

You don't want the exercise to repeat too many times, so next, you will add some code to stop `repetitions`{:class="block3variables"} from going above 5.

--- task ---

From the `Control`{:class="block3control"} blocks menu, select an `if ... then ... else`{:class="block3control"} block, and place the `change repetitions by 1`{:class="block3variables"} block in the space below `if ... then`{:class="block3control"}:

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
+ if <> then
    change [repetitions v] by (1)
else
+ end
```

--- /task ---

Now, you will add the condition `if`{:class="block3control"} `repetitions`{:class="block3variables"} `is less than`{:class="block3operators"} `5`.

**Note:** This sets the maximum number of repeats. You could choose a different number but the more repeats you allow, the longer the program takes to run.

--- task ---

From the `Operators`{:class="block3operators"} blocks menu, select a `less than`{:class="block3operators"} operator:

```blocks3
[]<[] ::operators
```

Place the block in the top space of the `if ... then ... else`{:class="block3control"} block, between `if`{:class="block3control"} and `then`{:class="block3control"}.

From the `Variables`{:class="block3variables"} blocks menu, take a rounded `repetitions`{:class="block3variables"} block and place it before the `<`{:class="block3operators"}. Type the number `5` after the `<`{:class="block3operators"}:

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators +> then
    change [repetitions v] by (1)
else
end
```

--- /task ---

Now, `repetitions`{:class="block3variables"} should only go up by `1` `if`{:class="block3control"} `repetitions`{:class="block3variables"} `is less than`{:class="block3operators"} `5`.

What will happen if the user sets `repetitions`{:class="block3variables"} to 5 or more?

--- task ---

Below `else`{:class="block3control"}, add a `say`{:class="block3looks"} block that will display the message `5 repetitions is the maximum` for `2` seconds:

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators> then
    change [repetitions v] by (1)
else
+     say [5 repetitions is the maximum] for (2) seconds
end
```

--- /task ---

Now, you need to do the same for the **down** arrow, but you need to use a different condition and reduce `repetitions`{:class="block3variables"} by 1 each time.

A way to say **reduce by 1** in Scratch is `change by`{:class="block3variables"} `-1`.

--- task ---

Select the **down** sprite. Add a `when this sprite clicked`{:class="block3events"} block and an `if ... then ... else`{:class="block3control"} block.

Add the condition `if`{:class="block3control"} `repetitions`{:class="block3variables"} `is more than`{:class="block3operators"} `1`.

Add a block so that if the condition is **true**, your program will `change repetitions by`{:class="block3variables"} `-1`.

Add a block so that if the condition is **false**, your program will `say`{:class="block3looks"} `Repetitions can't be lower than 1` for `2` seconds:

![Down arrow sprite icon](images/down_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions)>[1]> then
    change [repetitions v] by (-1)
else
    say [Repetitions can't be lower than 1] for (2) seconds
end
```

--- /task ---

Run the program to test it. Click on the two arrows to increase or reduce the number of repetitions.

Does `repetitions`{:class="block3variables"} stay between 1 and 5?

--- save ---
