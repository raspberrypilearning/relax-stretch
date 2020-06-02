## Getting your character ready

--- task ---
Open the Scratch starter project.

**Online**: open the starter project at [rpf.io/skiingon](http://rpf.io/skiingon){:target="_blank"}.

**Offline**: open the [starter project](http://rpf.io/sit-stretch-go){:target="_blank"} in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}.

In the starter project, you should see a character sprite along with two arrow, one up and one down.

![starter project](images/starter_project.png)

--- /task ---

First of all, you are going give **character 1** a name. In this project, she will be **Nadia** but you can use whatever name you like.

--- task ---

Select the **character 1** sprite in the **Sprites Pane**

Click on the _dialogue box_ showing the sprite name, and replace **character 1** with the name of your choice.

![select character 1 sprite name](images/select_character1_name2.png)

Click anywhere outside of the _dialogue box_ and you will see the name has now changed.

--- /task ---

Next, you will give **Nadia** all her setup code such as where on the screen start.

--- task ---

With the **Nadia** sprite still selected, add a `when flag clicked`{:class="block3events"} block from the list of `Events`{:class="block3events"} palette.

![character 1 sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
```

--- /task ---

--- task ---

Add a `go to x: y:`{:class="block3motion"} block from the `Motion`{:class="block3motion"} block palette.

Enter an **x value** of 70 and a **y value** of -25 to position **Nadia** low down to the right of centre.

![character 1 sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
+ go to x: (70) y: (-25)
```

--- /task ---

--- task ---

To make sure **Nadia** starts using the right costume, go to the `Looks`{:class="block3looks"} block palette and add a `switch costume to`{:class="block3looks"} block.

Set the costume to `at rest`{:class="block3looks"}.

![character 1 sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
+ switch costume to (at rest v)
```

--- /task ---

The last thing you'll do to prepare your **Nadia** is to add a short wait so that the first exercise doesn't start too suddenly.

--- task ---

Add a `Control`{:class="block3looks"} block to make **Nadia** `wait for 2 seconds`{:class="block3looks"} before anything else happens.

![character 1 sprite icon](images/nadia_sprite.png)

```blocks3
when flag clicked
go to x: (70) y: (-25)
switch costume to (at rest v)
+ wait (2) seconds
```

--- /task ---