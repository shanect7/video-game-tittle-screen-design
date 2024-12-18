# video-game-title-screen-design

## Video Game Title Screen Tutorial

Love video games? Hopefully you said yes because today's guide will guide you through the process of designing your own video game title screen.

## Table of Contents

// Anything after this point has NOT been worked on yet

// The table of contents has not been updated at all; change later

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [Step-by-Step Guide](#step-by-step-guide)
  - [1. Create the HTML File](#1-create-the-html-file)
  - [2. Create the CSS File](#2-create-the-css-file)
  - [3. Create the JavaScript File](#3-create-the-javascript-file)
  - [4. Link the CSS and JavaScript Files](#4-link-the-css-and-javascript-files)
  - [5. Open the HTML File in a Browser](#5-open-the-html-file-in-a-browser)
- [Things to Look Out For](#things-to-look-out-for)
- [Conclusion](#conclusion)

// idea A: You know that text that minecraft usually has? Can create design for that (to which they can write whatever text they want for that) 

// idea B: Can use Alpha Minecraft title screen or Beta Minecraft 

## Introduction

In this tutorial, you'll learn how to create a simple website with an HTML structure, styled with CSS, and interactivity added using JavaScript. By the end of this guide, you will have a basic understanding of how these three technologies work together to create a functional webpage.

For starters, you'll be learning how to code a simple functional title screen of the popular blocky video game (not Roblox), Minecraft! With the use of simple HTML structure and CSS styling, you'll be able to create a functioning title screen

// May need to mention: By the end, if you'd like, feel free to replace the images with your own or from the internet to create another video game title screen you like. (or perhaps even a video game of your own)

// TBD on if it's actually gonna be funcitoning 

## Objective

Use HTML links, images, headers, and CSS styling to match the final image of Minecraft's 2010 title screen:
![image](https://github.com/user-attachments/assets/e79f6df3-dd36-4ea1-b59f-48439d11b2db)

[Need to replace eventually; js a proof of concept for what it'll look like] 

## Project Structure

// Still need to adjust this 

Create a project directory and set up the following file structure:
```plaintext
simple-website/
├── index.html
├── styles.css
└── script.js
```
## Before starting...

Make sure that you have a folder/directory named "assets." This folder will have the images of all the buttons and backgrounds needed to design this title screen.

If now, you can copy and paste the "assets" folders from above into your repel/program.

## Step-by-Step Guide

### 1. Create and position the game title

Open your code editor and create a file named `index.html`. Add the following code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Website</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  Hello World!
  <script src="script.js"></script>
</body>
</html>
```
### 2. Create the CSS File

Create a file named `styles.css` and add the following code to style your webpage:

```css
body {
  font-family: Arial, sans-serif;
}
```

### 3. Create the JavaScript File

Create a file named `script.js` 

### 4. Link the CSS and JavaScript Files

Ensure that the CSS and JavaScript files are linked correctly in your `index.html` file. The `<link>` tag for CSS should be inside the `<head>` section, and the `<script>` tag for JavaScript should be just before the closing `</body>` tag.

### 5. Open the HTML File in a Browser

Open your `index.html` file in a web browser to see your simple website in action. You should see a styled heading, a paragraph, and a button that displays an alert when clicked.

## Things to Look Out For

- Ensure the file paths in the `<link>` and `<script>` tags are correct.
- Use proper HTML structure and semantics.
- Keep your CSS organized and use meaningful class names.
- Avoid inline styles and JavaScript as much as possible for better maintainability.
- Test your website in different browsers to ensure compatibility.

## Stretch Goals
If you finish early, feel free to try out these additions to your website!

### 6. Make it a Header!
Enclose the "Hello World!" in an ``<h1>`` tag as shown here:
```<h1> Hello World! </h1>```
<br>
The full code should now look like this:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Website</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1> Hello World! </h1>
  <script src="script.js"></script>
</body>
</html>
```


## Conclusion

Congratulations! You've created a simple website using HTML, CSS, and JavaScript. This is just the beginning – there are many more features and technologies to explore. Keep learning and experimenting to build more complex and dynamic websites.

Feel free to reach out if you have any questions or feedback. Happy coding!
