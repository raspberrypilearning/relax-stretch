## Adding control to buttons

Now let's code the arrow buttons to change the value of `repetitions`{:class="block3variables"} whenever they are clicked.

--- task ---

Leaving the existing code as it is. Grab a `when this sprite clicked`{:class="block3events"} block.

Add a `change repetitions by 1`{:class="block3variables"} variable block below that.

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
change [repetitions v] by (1)
```

--- /task ---

Click the green flag to test that `repetitions`{:class="block3variables"} goes up each time you click it.

Keep going. Does `repetitions`{:class="block3variables"} ever stop going up?

You don't want the exercise repeating 10,000 times, so let's add some code to stop `repetitions`{:class="block3variables"} going higher than 5.

--- task ---

Add an `if... then... else...`{:class="block3control"} block, placing your `change repetitions by 1`{:class="block3variables"} in the space below `if... then`{:class="block3control"} . 

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
+ if <> then
    change [repetitions v] by (1)
else
+ end
```

--- /task ---

You are going to add the _condition_ `if`{:class="block3control"} `repetitions`{:class="block3variables"} `is less than`{:class="block3operators"} `5`.

--- task ---

Drag a `less than`{:class="block3operators"} operator into top space of the `if... then... else...`{:class="block3control"} block.

Add a rounded `repetitions`{:class="block3variables"} block before the `<`{:class="block3operators"} and type the number `5` after it.

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators +> then
    change [repetitions v] by (1)
else
end
```

--- /task ---

Now, `repetitions`{:class="block3variables"} should only go up `1` `if`{:class="block3control"} `repetitions`{:class="block3variables"} `is less than`{:class="block3operators"} `5`, so now add what happens if `repetitions`{:class="block3variables"} is `5 or more`.

--- task ---

Add a say {:class="block3Looks"} block with the message "5 repetitons is the maximum" for `2` seconds.

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

Now you'll need to repeat these steps for the **down arrow**, but with a different _conditional statement_, reducing `repetitions`{:class="block3variables"} by `1` and giving a different message if the _condition_ is `false`.

--- task ---

Select the **down arrow** sprite, add a `when this sprite clicked`{:class="block3events"} event and an `if... then... else...`{:class="block3control"} block.

![Down arrow sprite icon](images/down_arrow_sprite.png)

```blocks3
when this sprite clicked
if <> then
else
end
```

--- /task ---

--- task ---

Make a block for the condition. You will need to add a `repetitions`{:class="block3variables"} block to a `is greater than 1`{:class="block3operators"} block. Look carefully for the `>` operator.

```blocks3
<(repetitions)>[1]>
```

Add this new _condition_ to your `if... then... else...`{:class="block3control"} block.

![Down arrow sprite icon](images/down_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions)>[1] ::operators +> then
else
end
```

--- /task ---

--- task ---

In the first empty space of the `if... then... else...`{:class="block3control"} block, add a block to reduce the `repetitions`{:class="block3variables"} by `1`.

![Down arrow sprite icon](images/down_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions)>[1]> then
+     change [repetitions v] by (-1)
else
end
```

**Note** that a way to say _reduce by 1_ in Scratch is, _change by -1_.

--- /task ---

Finally, add a message for if the **down arrow** is pressed but `repetitions`{:class="block3variables"} is already 1 and cannot go any lower.

--- task ---

In the `if... then... else...`{:class="block3control"} block, below `else`{:class="block3control"} add a say {:class="block3Looks"} block with the message "Repetitions can't be lower than 1" for `2` seconds.

![Down arrow sprite icon](images/down_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions)>[1]> then
    change [repetitions v] by (-1)
else
+     say [Repetitions can't be lower than 1] for (2) seconds
end
```

--- /task ---

Test your new code by running the program and clicking the two arrows to raise or reduce the number of repetitions. You may want to display the `repetitions`{:class="block3variables"} variable for the test so you can see the value of `repetitions`{:class="block3variables"} changing. To do this, _tick_ the variable's checkbox in the `variables`{:class="block3variables"} palette. 

![Making the repetition variable display on the stage](images/untickRepetitionsVariable.png)
