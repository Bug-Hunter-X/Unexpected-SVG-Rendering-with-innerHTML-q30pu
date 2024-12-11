# Unexpected SVG Rendering with innerHTML

This repository demonstrates an uncommon bug related to unexpected behavior when embedding SVG elements within HTML using the `innerHTML` property.  The SVG element, when inserted this way, might fail to render correctly or cause layout issues. This is due to the way innerHTML parses and interprets the inserted content.  The solution offers an alternative that avoids this unexpected behavior.

## Bug Description:

The provided HTML attempts to add an SVG circle to a div using `innerHTML`.  The SVG may fail to render completely or as intended, possibly displaying as a broken image or not at all.

## Solution:

The solution avoids using `innerHTML` for the SVG element. Instead, it creates the SVG element using DOM manipulation, preventing the rendering issues.

## How to Reproduce the Bug:

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the unexpected rendering or missing SVG element.

## How to Test the Solution:

1. Open `bugSolution.html` in a web browser.
2. Observe the correctly rendered SVG circle.