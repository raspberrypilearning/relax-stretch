## Getting the arrows ready

The next step is to *initialise* the arrow button sprites in the same way you have just done for the **Nadia** sprite.

--- task ---

Select the **up arrow** sprite in the **Sprites Pane** and give it a `when flag clicked`{:class="block3events"} block.

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
```

--- /task ---

--- task ---

Give the **up arrow** sprite a position on the Stage. Go to `Motion`{:class="block3motion"} and select the `go to`{:class="block3motion"} block. Type in x: `-140` and y: `30`.

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
+ go to x: (-140) y: (30)
```

--- /task ---

When the completed program runs, the **up arrow** can be clicked to increase the number of exercise repetitions. Since it is really easy to accidentally drag the button instead of just clicking it, use a `forever`{:class="block3control"} loop to make sure the sprite jumps straight back to its position.

--- task ---

Go to `Control`{:class="block3control"} in the Blocks palette, select a `forever`{:class="block3control"} loop and place it under the `green flag`{:class="block3events"} Event, with the `go to`{:class="block3motion"} block inside.

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
+ forever
go to x: (-140) y: (30)
+ end
```

--- /task ---

Next, you will do the same for the **down arrow** but this time you will place the sprite in a different position.

--- task ---

For the **down arrow** sprite, add a `green flag`{:class="block3events"} *event*, a `forever`{:class="block3control"} loop and a `go to`{:class="block3motion"} block.

Set the position in `go to`{:class="block3motion"} block to `x: -140` and `y: -40`

![down arrow sprite icon](images/down_arrow_sprite.png)

```blocks3
when flag clicked
forever
    go to x: (-140) y: (-40)
end
```

--- /task ---

Later, you'll add code to make these two buttons control the number of exercise repetitions but next, you'll code your first exercise routine.
