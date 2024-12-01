## Line-height as number override issue

This repository demonstrates a CSS bug where the `line-height` property, when specified as a pure number or with `rem` units, does not work as expected when overriding styles declared in an ancestor element.

### Bug Demonstration

The `bug.css` file showcases the problem. The `body` element sets a default font and `line-height`. When trying to override the `line-height` in a `div` without also setting the `font-size`, an unexpected result occurs.  The `line-height` does not change to the desired value.

### Solution

The `bugSolution.css` file provides the correct way to override the `line-height` property. By setting the `font-size` as well, the line-height applies correctly.