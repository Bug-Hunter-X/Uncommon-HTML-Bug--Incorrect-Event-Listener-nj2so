# Uncommon HTML Bug: Incorrect Event Listener

This repository demonstrates a subtle bug related to adding event listeners in JavaScript within an HTML file. The issue arises from incorrectly providing a string as the second argument to `addEventListener` instead of a function reference.

## Bug Description

The `bug.html` file contains a `div` element with an event listener attached using `addEventListener`.  However, instead of passing the `myFunction` function as the second argument, a string ("myFunction") is passed. This will not attach the event listener correctly.

## Bug Solution

The corrected code is in `bugSolution.html`. It shows the proper way to attach the event listener by passing a reference to the function `myFunction`. 

## How to reproduce:
1. Open bug.html in your browser. Click on the div element. You'll notice that no alert appears. 
2. Open bugSolution.html. Click on the div element. This time, the alert 'Div clicked!' will appear as expected.