# Uncommon HTML/JavaScript Error: Accessing Non-Existent Element

This repository demonstrates a subtle error that can occur in HTML and JavaScript when interacting with the DOM.
The primary issue lies in attempting to access properties or methods of elements that may not exist before they are checked.

## Bug Description:
The `bug.html` file contains JavaScript code that uses `document.querySelectorAll` and `document.querySelector` to select elements.
However, it does not check whether the selected elements actually exist before attempting to modify their styles.
This leads to an error in the console and unexpected behavior.

## Solution:
The `bugSolution.html` file corrects this by checking the existence of the element before accessing its properties.
This prevents the error and makes the code more robust.

## How to reproduce the bug:
1. Open `bug.html` in a web browser.
2. Observe the error message in the browser's developer console.
3. The text should remain visible, instead of being hidden.

## How to test the solution:
1. Open `bugSolution.html` in a web browser.
2. Observe that there is no error in the console.
3. The text should be hidden if '.myClass' is present, else remain visible.
