## Arrow button controls

Now it is time to code your arrow buttons so you can use them to change the value of `repetitions`{:class="block3variables"} while the program is running.

--- task ---

Leaving the existing code exactly as it is, add a new script starting with the `Events`{:class="block3events"} block, `when this sprite clicked`{:class="block3events"}.

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
+ when this sprite clicked
```

--- /task ---

--- task ---

Now add an `if... then... else...`{:class="block3control"} block from the `Control`{:class="block3control"} palette

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
+ if <> then
else
end
```

--- /task ---

The first thing you will add to the conditional `if... then... else...`{:class="block3control"} block is the _conditional statement_, `if`{:class="block3control"} block `repetitions`{:class="block3variables"} block `is less than 5`{:class="block3operators"}.

--- task ---

Start by dragging a `less than`{:class="block3operators"} block from the green `Operators`{:class="block3operators"} palette.

```blocks3
<()<()>
```

In first empty field, add a rounded `repetitions`{:class="block3variables"} block.

```blocks3
<(repetitions)<()>
```

In the remaining empty field, add the number `5`.

```blocks3
<(repetitions ::variables)<[5]>
```

Now add this block into the hexagonal field of your `if... then... else...`{:class="block3control"} block.

![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <(repetitions ::variables)<[5] ::operators +> then
else
end
```

--- /task ---

There are two remaining empty spaces in the `if... then... else...`{:class="block3control"} block. The first is for `if`{:class="block3control"} the _conditional statement_ `repetitions`{:class="block3variables"} block `is less than 5`{:class="block3operators"} is `true`, i.e. `repetitions`{:class="block3variables"} equals 4 or less. The second is for `if`{:class="block3control"} the _condition_ is `false`, e.g. `repetitions`{:class="block3variables"} equals 5 or more.

This means that `repetitions`{:class="block3variables"} can never go above `5`.

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

Since `repetitions`{:class="block3variables"} can't go above `5`, you can add a message for when a user presses the up button `repetitions`{:class="block3variables"} can't go higher.

--- task ---

Inside the empty space below the `else`{:class="block3control"} of the `if... then... else...`{:class="block3control"} block, add  the message `5 repetitons is the maximum`{:class="block3variables"} for `2` seconds.

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

Make up a block for the condition, `repetitions`{:class="block3variables"} block `is greater than 1`{:class="block3operators"}.

<(repetitions)>[1]>

Add this _condition_ to your `if... then... else...`{:class="block3control"} block.

```blocks3
when this sprite clicked
if <(repetitions)>[1] ::operators +> then
else
end
```

--- /task ---

--- task ---

In the first empty block space of the `if... then... else...`{:class="block3control"} block, i.e. `if`{:class="block3control"} the condition is `true`, add a block to reduce the `repetitions`{:class="block3variables"} by `1`.

```blocks3
when this sprite clicked
if <(repetitions)>[1]> then
+     change [repetitions v] by (-1)
else
end
```

**Note** that a way to say _reduce by 1_ in Scratch is, _change by -1_.

--- /task ---
