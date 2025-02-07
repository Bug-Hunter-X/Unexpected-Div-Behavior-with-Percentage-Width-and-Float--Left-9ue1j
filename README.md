# Unexpected Div Behavior with Percentage Width and Float: Left

This repository demonstrates a subtle CSS bug involving percentage widths, floating, and undefined parent container widths.  The bug manifests as unexpected collapsing of divs when the parent container lacks an explicit width declaration.

## Bug Description

The CSS rule `width: 50%; float: left;` on a `div` element is intended to make the div occupy 50% of its parent container's width and float to the left. However, if the parent container's width is not explicitly set, the divs will collapse or behave unexpectedly in some browsers because the percentage width is relative to the parent, and an undefined parent width leads to an inaccurate calculation.

## Bug Solution

The solution involves explicitly setting the width of the parent container. This ensures the percentage width of the child divs is correctly calculated.