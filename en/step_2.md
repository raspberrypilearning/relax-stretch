## Getting your character ready

--- task ---
Open the Scratch starter project.

**Online**: open the starter project at [rpf.io/sit-stretch-go](http://rpf.io/sit-stretch-go){:target="_blank"}.

**Offline**: open the [starter project](http://rpf.io/sit-stretch-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}.

In the starter project, you should see a character sprite along with two arrows, one up and one down.

![starter project](images/starter_project.png)

--- /task ---

Let's give **character 1** a name.

--- task ---

Select the **character 1** sprite.

Click on the _dialogue box_ showing the sprite name, and replace **character 1** with the name of your choice, e.g. **Nadia**.

![select character 1 sprite name](images/select_character1_name2.png)

--- /task ---

Next, you will give **Nadia** setup blocks such as `position`{:class="block3motion"} on the Stage.

--- task ---

With the **Nadia** sprite still selected, go to `Events`{:class="block3events"} in the Blocks palette and add the `when flag clicked`{:class="block3events"} block.

From the `Motion`{:class="block3motion"} block palette, add a `go to x: y:`{:class="block3motion"} block.

For **x**, enter an value of `70` and for **y**, enter a value of `-25`. This will position **Nadia** to the bottom right of the Stage.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
```

--- /task ---

--- task ---

At the start, **Nadia** needs to use the correct costume. Go to `Looks`{:class="block3looks"} in the Blocks palette and add a `switch costume to`{:class="block3looks"} block.

Set the costume to `at rest`{:class="block3looks"}.

Add a `wait for 2 seconds`{:class="block3looks"} so that the first exercise doesn't begin too suddenly.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
+ switch costume to (at rest v)
+ wait (2) seconds
```

--- /task ---
