## Getting the arrows ready

The next step is to *initialise* the arrow button sprites in the same way you have just done for the *character 1* sprite.

--- task ---

Select the **up arrow** sprite in the **Sprites Pane** and give it a `when flag clicked`{:class="block3events"} block.

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
```

--- /task ---

--- task ---

Give the **up arrow** sprite the screen position `x: -140` and `y: 30` by adding a `go to`{:class="block3motion"} block.

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
+ go to x: (-140) y: (30)
```

--- /task ---

When the finished program is running, the **up arrow** will be clicked to increase the number of exercise repetitions. Since it is really easy to accidentally drag the button instead of just clicking it, use a `forever`{:class="block3control"} loop to make sure the sprite jumps straight back to its position.

--- task ---

Since the **up arrow** is 

Give the **up arrow** sprite the screen position `x: -140` and `y: 30` by adding a `go to`{:class="block3motion"} block.

![up arrow sprite icon](images/up_arrow_sprite.png)

```blocks3
when flag clicked
+ forever
    go to x: (-140) y: (30)
end
```

--- /task ---