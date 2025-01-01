# CSS Specificity Bug

This repository demonstrates a common CSS specificity issue where a seemingly simple selector fails to apply to all intended elements. The bug involves unexpected styling of list items in an unordered list, affecting only the first item.

## Bug Description
The provided `bug.css` file contains a CSS rule intended to style all list items (`<li>`) within an unordered list (`<ul>`). However, due to CSS selector specificity, only the first list item receives the styling.  This is often due to other, more specific selectors overriding the general rule.

## Solution
The solution is provided in `bugSolution.css`. To solve the issue, more specific styles should be examined. Sometimes, using the `!important` flag is a quick fix, but this isn't generally recommended as it can lead to future maintenance problems. Proper use of cascading and specificity should be prioritized.