# Video Game Title Screen

## What are we doing?

In this project, we'll be rebuilding the Minecraft Java Edition (AKA: the better edition) title screen with actual Minecraft assets 

![](https://github.com/shanect7/video-game-tittle-screen-design/blob/main/custom_designed_final_menu.gif)


## Section 1: The Background and Title
To start off, we will be uploading one of Minecraft's title screen background images. (And, to make it easier for ourselves, it will already have the title on it)

Starting in 'index.html' we will be creating a division, or section, to "hold" our background image. With the `<div>` tag, we will be creating it with the class "bg" inside the body element.

Such should look like this:

```
<body>
  <div class="bg">
  </div>
</body>
```

With that done, we will now be going into `styles.css` to use 'bg' class to showcase our background image. Within this class, we will be using the following format to alter the class and add a background-image

We will be starting with this:
```
.bg {

    /* flex container for child elements (AKA: the buttons) */
    display: flex; 
    flex-direction: column;
    justify-content: center;
}
```

Note: The code already in there will be used later to create our buttons

To add our background, we will have to use the `background-image` property within the 'bg' class.

Once that is completed, you will find that the background looks off, sort of like this:
![image](https://github.com/user-attachments/assets/733d269a-1e66-4884-b28a-375e0efb1a3a)

Unfortunately though, most players wouldn't be satisfied with seeing only half the title and background screen, which means more work for us. So, to this fix this, we will be using the following CSS properties:

`background-position:` 
This property determines the position of the background image.

For our title screen, it'd be ideal to use a property to <ins>**center**</ins> it on the screen.

`background-size:`
This property determines the size of the background image. 

To make sure the background image fits across the entire scene, we'd like to use a background-size property that <ins>**cover**</ins>s the entire screen.

`background-repeat:` 
This property determines if a background image should repeat over and over again across the screen. (This is more visible within images that are small) 

While our background image will likely not repeat, it would still be good to ensure it doesn't. Luckily, a property for <ins>**no-repeat**</ins>ing does exist.

With all those properties in place, we will be left with the following:
![image](https://github.com/user-attachments/assets/e713ab5a-827c-441a-98eb-543d8a3e5286)

## Section 2: The Buttons
With our background and title now created, we will now be focusing on the creation of our buttons.

Starting off with 'index.html' again, we will be using the `<div>` HTML tag to create two new divisions with classes named "center_buttons" and "bottom_buttons" within the division with the class name "bg."

It should look something like this
```
<body>
  <div class="bg">
      <div class="center_buttons">
      </div>
      <div class="bottom_buttons">
      </div>
  </div>
</body>
```

Now that we have our divisions set up, we will now be inputting some images inside these divisions that represent our buttons, all inside 'index.html'

With the use of the `<img>` HTML tag, we will be using the images within the 'minecraft-assets' folder to set up our button images. 

To help you out, one example of the use of the `<img>` tag within our code will look like this:
```
  <img src="minecraft-assets/singleplayer_button.png" alt="Singleplayer Button">
```

The `<img>` tag requires showing the path to the image we want to use, which happens to be in the minecraft-assets folder. In addition to that, the `<img>` tag allows you have to alternative text, designated by: `alt="[text here]"` that will be shown if your picture doesn't show up. The use of the alt. text is useful, especially when debugging your code, as it shows up when the code itself works but the image itself is not showing up. 

With all that in mind, please place images under the proper division. 

The divisions should have the following images:

**Center Buttons:**

• Singleplayer Button

• Multiplayer Button

• Minecraft Realms Button

**Bottom Buttons:**

• Language Button

• Options Button

• Quit Button

• Accessibility Button

Note: For the title screen to look right, the images must be added in this order 

When you have completed all that, you will be left with a title screen that looks like this:
![image](https://github.com/user-attachments/assets/4c3e31aa-f665-46af-a17d-fbc2d8e1a7b8)

For a game that (seriously) costs $30, most players would expect a much cleaner and organized main menu screen, so let's fix this up!

In `styles.css` we will be styling the "center_buttons" class first. With that in mind, start by creating the selector:
```
.center_buttons {

}
```

Once that is done, then, inside the selector (or the curly braces), type ``display: flex;``. Such will tell our buttons that we'll be using the flexbox model to organize it. 

Since these buttons have spacing between them, you'll also want to use the ``gap`` property. Within the selector (or curly braces) also type ``gap: 10px;``

With that done, we will then have to use our knowledge of the flexbox model to <ins>**center**</ins> and place the buttons in a <ins>**column**</ins> format. 

Once you have figured that out, you should be left with a main menu screen that looks like this:

![image](https://github.com/user-attachments/assets/66ab24ef-d59c-434d-92fd-08ee382f5a1b)

We're almost done! With that completed, we will now be doing the same thing for the "bottom_buttons." Create another selector using the bottom_buttons class. Also, like the center_buttons, you'll need to establish a flexbox model, a gap, and now a new property called ``margin-top.``

The following should look like this:
```
.bottom_buttons {
  display: flex; 
  gap: 10px; 
  margin-top: 40px;
}
```

With that all written, you must now consider what else about this flexbox model must be changed to <ins>**center**</ins> the buttons. 

And with that, we should have our final product, that being something like this!
![image](https://github.com/user-attachments/assets/05b57169-bd56-4a0b-94c9-a5a5a755b2d3)

## (Stretch Goal) Section 3: Animated Text
NOTE: This is optional! (I will be showing you something you have not learned yet) 

On the main menu of Minecraft you'll notice that flashing yellow text right by the title. Such text is called "splash text."

In order to recreate this we will create a `<div>` called "splash_text" within the `<div>` with the class named 'bg.' And, then within this new `<div>` you will then use the `<p>` tag to create your own custom text.
```
<body>
  <div class="bg">
      <div class="splash_text">
      </div>
      <div class="center_buttons">
        ...
      </div>
      <div class="bottom_buttons">
        ...
      </div>
  </div>
</body>
```

You will then end up with something like this:
![image](https://github.com/user-attachments/assets/d0f361e3-e1ac-4ebe-9eb2-fdc89bd7d80c)

With our text now created, we should then head to `styles.css` Within our CSS, we will start by importing a custom font to match the real Minecraft menu. With the use of a CSS at-rule (AKA: @ statements that instructs how the CSS should behave), @font-face will display a custom font with the use of:

`font-family:`
Specifies a list of fonts to use. 

Inside font-family, within the use of quotation marks, it will designate a name to your own custom font. 
[More info. on font-family here](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)

Within our CSS, you should type out the following: (ideally, under the code you've made earlier) 
```
  @font-face {
    font-family: 'minecraftregular';
    src: url('https://fonts.cdnfonts.com/s/25041/1_MinecraftRegular1.woff') format('woff');
}
```

(For more information on @font-face, consider this [website](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face))

Following that, with the use of the "splash_text" class, we will now apply this custom font to our text, like shown below: 
```
.splash_text {
  font-family: 'minecraftregular', sans-serif;
}
```

As you can see their a comma placed in between our custom font and sans-serif. We do this in order to have a back-up font in case our custom font doesn't work. Like a list, the displayed font prioritizes from first to last font (left to right in this case). If the first font fails to display, it will move on to the font on its right. 

With that now completed, we will now focus on the size of this font. In order to change the size of this text, we will now use `font-size` which is based on pixels. 
[More info. on font-size here](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)

Should look like this:
```
.splash_text {
  font-family: 'minecraftregular', sans-serif;
  font-size: 30px;
}
```

We will also now add a new color and text-shadow to our splash text.

In order to do this, we will use:

`color`

AND

`text-shadow`

Such property can hold up to four values, as designated below:
```
text-shadow: offset-x, offset-y, blur-radius, color */
```

The offsets will adjust position of the shadow horizontally (x) and vertically (y) while the blur-radius, adjusts how blurry the shadow is. 

In our case though, we will not be using the blur-radius value, so we will omit that in our final code. 

All in all, it should look like this:
```
.splash_text {
  font-family: 'minecraftregular', sans-serif;
  font-size: 30px;
  color:#fafd11;
  text-shadow: 1px 2px #463903;
}
```

With that all completed, we will now be altering the position and animation of the text. Since this is all complex, please use the following properties and juse use the code listed below:

`position`
`animation`
`top`
`left`
`@keyframes`
`transform`

```
.splash_text {
  font-family: 'minecraftregular', sans-serif;
  font-size: 30px;
  color:#fafd11;
  text-shadow: 1px 2px #463903;
  position:absolute;
  animation:text .5s linear infinite normal;
  top: 60px;
  left: 800px;
  /* transform rotate will affect position */
}

top: 125px;
left: 828px;
@keyframes text {
  0% {
    transform:scale(1) rotate(-30deg);
  }
  50% {
    transform:scale(0.9) rotate(-30deg);
  }
  100% {
    transform:scale(1) rotate(-30deg);
  }
}
```

And with that, we have our final main menu screen!

