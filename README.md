# CSS `calc()` Issue with Padding and Borders

This repository demonstrates a common error when using the `calc()` function in CSS to calculate widths, particularly when dealing with parent elements that have padding or borders. The issue arises because `calc()` doesn't automatically account for these elements.  This can lead to unexpected and inconsistent layout behavior.

The `bug.css` file illustrates the problem. The `solution.css` file provides a corrected implementation.

## Reproducing the Bug

1. Open `bug.html` in a web browser.
2. Observe the width of the inner element.  It will be smaller than expected.

## Solution

The solution involves explicitly subtracting the parent's padding and border from the calculation within `calc()`.  See `solution.css` for the corrected code.