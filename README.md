# Video Game Title Screen

## What are we doing?

In this project, we'll be rebuilding the Minecraft Java Edition (AKA: the better edition) title screen with actual Minecraft assets 

![image](https://github.com/user-attachments/assets/2f5bd731-9271-41e0-acdb-b31dec0a8652)
(CHANGE IMAGE LATER, PLACEHOLDER)

## Step 1: The Background and Title
To start off, we will be uploading one of Minecraft's title screen background images. (And, to make it easier for ourselves, it will already have the title on it)

Now, in `styles.css` we will be using the 'bg' class to showcase our background image. Within this class, we will be using the following format to alter the class and add a background-image

We will be starting with this:
```
.bg {

}
```

Note: The class 'bg' is a 'div' made in `index.html` to style in CSS

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

Answer: (Will remove once students see this, just here for my use)
```
/* the .bg refers to the 'bg' div in index.html*/
  .bg {
    /* The image used */
    background-image: url('minecraft-assets/minecraft_background_with_title.png');
  
    /* Full height */
    height: 100%;
  
    /* Center and scale the image nicely */
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
  }
```

## Step 2: The Buttons
With 


[Remove later]
HTML Answer:
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="styles.css">
    <title>Minecraft Main Menu</title>
  </head>
<body>
  <div class="bg">
    <div class="center_buttons">
      <img src="minecraft-assets/singleplayer_button.png" alt="Singleplayer Button">
      <img src="minecraft-assets/multiplayer_button.png" alt="Multiplayer Button">
      <img src="minecraft-assets/minecraft_realms_button.png" alt="Minecraft Realms Button">
      </div>
    <div class="bottom_buttons">
      <img src="minecraft-assets/language_button.png" alt="Language Button">
      <img src="minecraft-assets/options_button.png" alt="Options Button">
      <img src="minecraft-assets/quit_button.png" alt="Quit Button">
      <img src="minecraft-assets/accessibility_button.png" alt="Accessibility Button">
    </div>
  </div>
</body>
</html>

CSS Answer:
body, html {
    margin: 0;
    height: 100%; 
    display: flex; 
    flex-direction: column;
  }
  /* Leave the above on top*/
  
  /* the .bg refers to the 'bg' div in index.html*/
  .bg {
    background-image: url('minecraft-assets/minecraft_background_with_title.png');
    height: 100%;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;  

    /* Flex container for child elements */
    display: flex; 
    flex-direction: column;
    justify-content: center;
  }

  .center_buttons {
    display: flex; 
    align-items: center;
    flex-direction: column;
    gap: 10px; 
}   

/* Note: align-items: row not needed for images automatically placed in a row */

.bottom_buttons {
  display: flex; 
  justify-content: center;
  gap: 10px; 
  margin-top: 10px;
}   

