# Animated Proposal Webpage

## Overview

This project showcases a simple and interactive animated proposal webpage. The webpage includes a charming header, an animated GIF, and two buttons: "Yes" and "No." The "No" button adds an engaging touch by moving randomly across the screen when clicked or hovered over.

## Key Features

- **Engaging Animation:** The webpage includes a dynamic GIF to capture attention and add a playful element to the proposal.
  
- **Interactive Buttons:** Users can respond to the proposal by clicking the "Yes" button, which triggers a redirection to the "yes.html" page. The "No" button, when clicked or hovered over, dynamically moves to a random position on the screen, creating an amusing effect.

## JavaScript Functions

The JavaScript functions in the code control the interactive behavior of the webpage:
- **`nextPage()`:** Redirects the user to the "yes.html" page when the "Yes" button is clicked.
  
- **`moveButton()`:** Dynamically moves the "No" button to a random position within the window, either when clicked or hovered over.

Explore the [HTML source code](index.html) to understand the implementation details and customize the proposal webpage according to your preferences.

## JavaScript Functions
 ```javascript
function nextPage() {
            window.location.href = "yes.html";
        }

        function moveButton() {
            var x = Math.random() * (window.innerWidth - document.getElementById("noButton").offsetWidth);
            var y = Math.random() * (window.innerHeight - document.getElementById("noButton").offsetHeight);
  
            document.getElementById("noButton").style.left = `${x}px`;
            document.getElementById("noButton").style.top = `${y}px`;
        }
```

## Usage

1. Clone the repository.
2. Open the index.html file in your web browser.
3. Experience the interactive proposal webpage.
 
Feel free to customize the content and styles according to your preferences.

## Demo

Check out the live demo [here](https://shivoham8.github.io/doyouwannagooutwithme/).

## Note

This project is created for playful and illustrative purposes. Enjoy the interaction!
