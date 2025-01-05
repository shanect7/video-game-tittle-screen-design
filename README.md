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

Note: The class 'bg' is a 'div' made in `index.html` to style in css

To add our background, we will have to use the `background-image` property within the 'bg' class.

Once that is completed, you will find that the background looks off, sort of like this:

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
