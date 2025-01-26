# Uncommon HTML Bug: Premature DOM Manipulation

This repository demonstrates a common yet subtle error in HTML and JavaScript interaction. The bug involves attempting to manipulate the DOM (Document Object Model) before the elements are fully loaded and parsed by the browser.  This often leads to runtime errors or unexpected behavior.

## Bug Description

The `bug.html` file contains a script that tries to modify the `innerHTML` property of a div element before the element is fully rendered in the DOM.  This results in a JavaScript error because the element is not found.

## Solution

The solution in `bugSolution.html` uses the `DOMContentLoaded` event listener.  This ensures that the script executes only after the HTML document is completely parsed, preventing the error.