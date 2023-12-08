# Keep Awake Script

## Overview
This repository contains a simple HTML, CSS, and JavaScript script that simulates typing in a text box. This script is designed to potentially keep your computer from going to sleep.

## How It Works
The script types the text "Keeping your system awake..." into a text area, one character per second. When it reaches the end of the string, it clears the text area and starts over.

## Usage
To use this script, simply open the HTML file in your web browser.

## Code
Here is the main JavaScript function that powers the script:

```javascript
var textArea = document.getElementById('keepAwake');
var text = "Keeping your system awake...";
var index = 0;

function typeText() {
    if(index < text.length) {
        textArea.value += text.charAt(index);
        index++;
    } else {
        textArea.value = '';
        index = 0;
    }
}

setInterval(typeText, 1000); // types a character every second
```

## Disclaimer
Please note that this is a very basic implementation and might not work in all scenarios or on all systems. It's always best to adjust your system's power settings if you need to keep it awake for extended periods. Also, be aware that keeping your system awake can consume more power and potentially shorten the lifespan of your hardware. Use this responsibly!

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
```

This README provides an overview of the project, explains how the script works, provides usage instructions, and includes a disclaimer. It's always a good idea to include a license for your project as well. 😊
