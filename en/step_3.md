## Getting the arrows ready

The next step is to *set up* the arrow button sprites in the same way you have just done for the **Nadia** sprite.

--- task ---

Select the **up arrow** sprite and give it a `when flag clicked`{:class="block3events"} block.

Add a `go to`{:class="block3motion"} block, setting **x** to `-140` and **y** to `30`.

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
go to x: (-140) y: (30)
```

--- /task ---

When running the program, it is easy to accidentally drag the button instead of just clicking it! You could use a `forever`{:class="block3control"} loop around your `go to`{:class="block3motion"} block to make sure the sprite stays in its position.

--- task ---

Grab a `forever`{:class="block3control"} loop and place it under the `green flag`{:class="block3events"} with the `go to`{:class="block3motion"} block inside.

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
+ forever
go to x: (-140) y: (30)
+ end
```

--- /task ---

Now do the same for the **down arrow** but in a different position.

--- task ---

For the **down arrow** sprite, set the `go to`{:class="block3motion"} block values to **x** at `-140` and **y** at `-40`

![down arrow sprite icon](images/down_arrow_sprite.png)

```blocks3
when flag clicked
forever
    go to x: (-140) y: (-40)
end
```

--- /task ---

Later, you'll add code to make these two buttons control the number of exercise repetitions but next, you'll code your first exercise routine.
