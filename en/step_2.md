## Getting your character ready

--- task ---
Open the Scratch starter project.

**Online**: open the starter project at [rpf.io/sit-stretch-go](http://rpf.io/sit-stretch-go){:target="_blank"}.

**Offline**: open the [starter project](http://rpf.io/sit-stretch-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}.

In the starter project, you should see a character sprite along with two arrows: up and down.

![starter project](images/starter_project.png)

--- /task ---

Let's give **character 1** a name.

--- task ---

Select the **character 1** sprite.

Click on the _dialogue box_ showing the sprite name. We have named this sprite **Nadia**. Feel free to replace **character 1** with the name of your choice.

![select character 1 sprite name](images/select_character1_name2.png)

--- /task ---

Next, you will give **Nadia** setup blocks such as `position`{:class="block3motion"} on the Stage.

--- task ---

With the **Nadia** sprite still selected, add a `when flag clicked`{:class="block3events"} block.

Below that, add a `go to x: y:`{:class="block3motion"} block with **x** set to `70` and **y** to `-25`. 

Add a `switch costume to`{:class="block3looks"} block, setting the costume to `at rest`{:class="block3looks"}.

Lastly, add a `wait for 2 seconds`{:class="block3control"} so that the first exercise doesn't begin too suddenly.

![Nadia sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
switch costume to (at rest v)
wait (2) seconds
```

--- /task ---
