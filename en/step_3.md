## Prepare the arrows

The next step is to set up the arrow button sprites in the same way as you have just done for the **Nadia** sprite.

--- task ---

Select the **up arrow** sprite and give it a `when green flag clicked`{:class="block3events"} block.

Add a `go to`{:class="block3motion"} block, and set `x`{:class="block3motion"} to `-140` and `y`{:class="block3motion"} to `30`:

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
go to x: (-140) y: (30)
```

--- /task ---

When running the program, it is easy to accidentally drag the button instead of clicking it! To make sure that the sprite stays in its position, use a `forever`{:class="block3control"} loop around the `go to`{:class="block3motion"} block. 

--- task ---

Take a `forever`{:class="block3control"} loop and place it under the `when green flag clicked`{:class="block3events"} block, with the `go to`{:class="block3motion"} block inside:

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
+ forever
go to x: (-140) y: (30)
+ end
```

--- /task ---

Now, you will do the same for the **down arrow**, but in a different position.

--- task ---

For the **down arrow** sprite, set the `go to`{:class="block3motion"} block values to `x`{:class="block3motion"} at `-140` and `y`{:class="block3motion"} at `-40`:

![down arrow sprite icon](images/down_arrow_sprite.png)

```blocks3
when flag clicked
forever
    go to x: (-140) y: (-40)
end
```

--- /task ---

In a later step, you will develop the code for the two buttons so that they control the number of times that the exercises repeat themselves.

Next, you will code your first exercise routine.

--- save ---
