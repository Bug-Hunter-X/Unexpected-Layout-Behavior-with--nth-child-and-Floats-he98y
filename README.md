# CSS Layout Bug: Unexpected Behavior with :nth-child and Floats

This repository demonstrates a subtle but common bug in CSS layouts related to using the `:nth-child` selector to clear floats. The problem arises when trying to force a specific element to start on a new line, but the solution is overly dependent on the element's position.  This can lead to unexpected behavior if the DOM structure changes.

The `bug.css` file showcases the flawed approach, while `bugSolution.css` provides a more robust and maintainable solution.

## Reproducing the Bug

1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe the layout. Add or remove content before the second div to see how the layout breaks.

## Understanding the Solution

The solution avoids relying on `:nth-child` and uses clearer, more flexible methods such as clearing floats on their container element.