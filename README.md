#### Project Title: Inverto
#### Video Demo: https://youtu.be/tzcBwouTXD0
#### Description:

This is Inverto, a simple Chrome extension that inverts the colors on your webpage for a smoother browsing experience. On clicking the icon of the extension, the colors of the current webpage we're visitng are inverted. By using this feature, we can easily switch to dark mode to view things on the webpage more comfortably.


**appOn.js:**

This Javascript file is used to invert the color of a media element - which can be an image or video, and inverts the color of the text on the web page from light to dark. This is used to create the dark mode for our webpage.

**appOff.js:**

This Javascript file reverts the the theme from dark mode to light mode by inverting the colors that were already inverted by appOn.js. This also includes the media elements - images and videos as well as text.

**manifest.json:**

This file contains the manifest version of my Chrome extension as well as the desciption of the extension.

It also contains the images (in the .png format) required for display as the icon for the Chrome extension. I uploaded a 16x16, 48x48 and a 128x128 .png version of the image I chose as my icon. Permission to access the contents of the webpage as well as the active tab were also granted in this manifest.json file.
I looked up the guide on https://developer.chrome.com/docs/extensions/mv3/getstarted/ to help me get started with this.

**popup.html:**

In the .popup function, I made a popup appear that says "inverto". I set the background of the rectangular pop-up as lavenderblush. I made the logo of the extension in a bright coral color and handwritten font. I linked the font 'shadows into light' in the head tag by pasting the google fonts link into it. I then set the size of the popup to  minimum width 344px and height 188px. I also added the desciption of the extension in the paragraph tag of popup.html.

To enable intuitive switching between light and dark modes, i employed the use of a button that can be used as a switch. The button when slid from left to right enables dark mode and the color of the button changes from light coral to dark coral using the transformToCoral and transformToDarkCoral functions.

I made the space next to the button display "invert" before the button was slid to the right and display "revert" after the button was slid to the right.
I used the moveCircleleft and moveCircleRight functions to slide the button from left to right and dynamically change colors.

In the body of popup.html I set the size of the button as well as the alignment of the text that is next to the button and linked popup.js to popup.html

**popup.js:**

This is used to control the dynamic aspects of this extension. Here I defined a function invert() that was the function responsible for inverting the colors of images, videos and text on the webpage being viewed currently. i added an event listener to the button for a click on the button and that acts as a cue for the extension to invert colors. Using if-else conditons I implemented the inverting and reverting of the colors on the webpage.

**Here are some screenshots to demonstrate the working of my project:**


<img width="1440" alt="image" src="https://user-images.githubusercontent.com/77161873/178329958-0e6ce8c4-edc2-407e-8afa-9691f4dccef8.png">

<img width="392" alt="image" src="https://user-images.githubusercontent.com/77161873/178330007-7e24c002-6a55-4bff-b962-0564fa33c4ff.png">

<img width="1440" alt="image" src="https://user-images.githubusercontent.com/77161873/178330073-a1c7c1d0-e72f-4cb8-9b75-4b426ef9a759.png">

<img width="402" alt="image" src="https://user-images.githubusercontent.com/77161873/178330122-ef538b6e-2d94-465d-b99a-f6880327a460.png">


My main takeaway from this project:

I learnt how to create a Chrome extension by reading the documentation and watching a few helpful tutorials and used the concepts of HTML, CSS and JavaScript to create a Chrome Extension that dynamically inverts the display theme of any website. I also plan on publishing my extension when i improve it further. 
