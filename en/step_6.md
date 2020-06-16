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

You don't wan the exercise repeating 10,000 times, so let's add some code to stop `repetitions`{:class="block3variables"} going higher than 5.

--- task ---

Add an `if... then... else...`{:class="block3control"} block, placing your `change repetitions by 1`{:class="block3variables"} in the space below `then`{:class="block3control"} . 

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
+ if <> then
    change [repetitions v] by (1)
else
+ end
```

--- /task ---

You are going to add the _condition_ `if...`{:class="block3control"} `repetitions`{:class="block3variables"} `is less than 5`{:class="block3operators"}.

--- task ---

Drag a `less than`{:class="block3operators"} operator into top space of the `if... then... else...`{:class="block3control"} block.

Add a rounded `repetitions`{:class="block3variables"} block before the `<` and type the number `5` after it.

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators +> then
    change [repetitions v] by (1)
else
end
```

In the first empty field, add a rounded `repetitions`{:class="block3variables"} block.

```blocks3
<(repetitions)<()>
```

In the last empty field, add the number `5`.

```blocks3
<(repetitions ::variables)<[5]>
```

Now add this block into the hexagonal field of the `if... then... else...`{:class="block3control"} block.

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators +> then
else
end
```

--- /task ---

The first empty space (`if...`{:class="block3control"}) defines what happens if the _conditional statement_ is `true`. It is true if the number of repetitions is less than 5 (i.e. equal to or less than 4).

The second empty space (`else...`{:class="block3control"}) defines what happens when the _conditional statement_ is `false`. It is false if the number of repetitions is equal to or more than 5.

This will mean that `repetitions`{:class="block3variables"} can never go above `5`.

--- task ---

Inside the first empty space of the `if... then... else...`{:class="block3control"} block, add a `change repetitions by 1`{:class="block3variables"} to add `1` to the variable.

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators> then
+     change [repetitions v] by (1)
else
end
```

--- /task ---

The program will now stop `repetitions`{:class="block3variables"} from going above `5`. You need to add a message for a user.  If they try to press the up button above 5, the program will say "5 repetitons is the maximum".

--- task ---

Inside the `if... then... else...`{:class="block3control"} block, below the `else`{:class="block3control"} add a say {:class="block3Looks"} block with the message "5 repetitons is the maximum" for `2` seconds.

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
