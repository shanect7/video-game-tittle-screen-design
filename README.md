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

Unfortunately though, most players aren't typically satisfied with seeing only half the title and background screen, which means more work for us. So, to this fix this, we will be using the following CSS properties:

`background-position:` 
This property determines the position of the background image.

For our title screen, it'd be ideal to use a property to <ins>**center**</ins> it on the screen.

`background-size:`
This property determines the size of the background image. 

To make sure the background image fits across the entire scene, we'd like to use a background-size property that <ins>**cover**</ins>s the entire screen.

`background-repeat:` 
This property determines if a background image should repeat over and over again across the screen. (This is more visible within immages that are small) 

While our background image will likely not repeat, it would still be good to ensure it doesn't. Luckily, a property for <ins>**no-repeat**</ins>ing does exist.

To fix this, 
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
