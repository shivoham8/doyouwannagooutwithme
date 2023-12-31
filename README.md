# Animated Proposal Webpage

## Overview

This project showcases a simple and interactive animated proposal webpage. The webpage includes a charming header, an animated GIF, and two buttons: "Yes" and "No." The "No" button adds an engaging touch by moving randomly across the screen when clicked or hovered over.

## HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Proposal</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <div class="header_text">Do you wanna go out with me?</div>
        <div class="gif"><img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNThtMjludHR1ZTNzNjR0eWJ0c3h0M3RuNmc4aXl2Z3EwbG8waHpubSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/cLS1cfxvGOPVpf9g3y/giphy.gif" alt="animated-image"></div>
        <div class="buttons">
            <button class="btn" id="yesButton" onclick="nextPage()">Yes</button>
            <button class="btn" id="noButton" onmouseover="moveButton()" onclick="moveButton()">No</button>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>
```

## Javascript Structure
 ```
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
4. 
Feel free to customize the content and styles according to your preferences.

## Demo

Check out the live demo [here]().

## Note

This project is created for playful and illustrative purposes. Enjoy the interaction!
