# Uncommon HTML Bug: Accessing Non-Existent Properties

This repository demonstrates an uncommon bug in HTML that can occur when accessing properties of objects that are unexpectedly null or undefined.  The specific bug focuses on attempting to access a property of a DOM element that might not exist.

## Bug Description
The bug arises from the assumption that `document.getElementById('myDiv')` always returns a valid DOM element.  If the element with the ID 'myDiv' does not exist, this function will return `null`.  Attempting to access properties of a `null` object will cause an error.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. You should see a JavaScript error in your browser's console.

## Solution
The solution is to perform a null check before attempting to access any properties of the element:

## Solution Code (bugSolution.html)
The `bugSolution.html` file provides a corrected version of the code. It includes a null check to prevent the error:
