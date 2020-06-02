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
<(repetions ::variables +)<()>
```

In the remaining empty field, add the number `5`.

```blocks3
<(repetions ::variables)<(5 +)>
```


![Up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when this sprite clicked
if <> then
else
end
```

--- /task ---