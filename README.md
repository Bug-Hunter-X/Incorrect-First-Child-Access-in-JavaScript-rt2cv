# Uncommon HTML Bug: Incorrect First Child Access

This repository demonstrates an uncommon bug related to accessing the first child of an HTML element using JavaScript. The issue arises when assuming the first child is always an element node, when in fact it could be a text node (e.g., whitespace).  The solution provides the correct approach using `firstElementChild`.

## Bug
The bug lies in directly manipulating the `firstChild` property without checking its node type. This leads to unexpected errors or incorrect behavior if the first child is a text node.

## Solution
The solution uses `firstElementChild` to specifically target the first element child, avoiding the potential problems associated with text nodes.