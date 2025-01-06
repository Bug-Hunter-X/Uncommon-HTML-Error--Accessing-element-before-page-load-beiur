# Uncommon HTML Error: Accessing Element Before Page Load

This repository demonstrates a common yet often overlooked error in HTML: accessing and manipulating DOM elements before the page has fully loaded.  The issue often manifests as seemingly random errors or unexpected behavior.

## The Problem

The `bug.html` file contains JavaScript code that attempts to modify the content of a `div` element immediately after the script is executed.  If the page's parsing and rendering haven't completed yet, the element may not exist in the DOM, leading to a failure.

## The Solution

The `bugSolution.html` file addresses this by using `setTimeout` to delay the execution of the code that modifies the `div` element. This ensures that the page has enough time to fully load, preventing the error.