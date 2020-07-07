## Prepare your character

--- task ---

If working **online**, open the [starter project](http://rpf.io/p/en/sit-stretch-on){:target="_blank"} in Scratch.

If working **offline**, open the project [starter file](http://rpf.io/p/en/sit-stretch-get){:target="_blank"} in the Scratch offline editor. If you need to download and install Scratch, you can find it [here](https://scratch.mit.edu/download){:target="_blank"}.

You should see a character sprite along with two arrows: up and down.

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

Below that, add a `go to x: y:`{:class="block3motion"} block with `x`{:class="block3motion"} set to `70` and `y`{:class="block3motion"} to `-25`. 

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

--- save ---
