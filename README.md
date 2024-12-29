# CSS Calc() Function Syntax Error

This repository demonstrates a subtle syntax error in CSS's `calc()` function. The error arises from an unexpected space between the minus sign and the number within the calculation.

## Bug

The `bug.css` file contains the following CSS rule:

```css
#myElement {
  width: calc(100% - 50 px);
}
```

This code is incorrect because of the space between `-` and `50`.  The correct syntax requires no space. This seemingly minor error causes unexpected results.

## Solution

The corrected code is in `bugSolution.css`:

```css
#myElement {
  width: calc(100% - 50px);
}
```

This version removes the space, making the calculation work correctly.

## How to reproduce

1. Create an HTML file with an element with the id "myElement".
2. Link either `bug.css` or `bugSolution.css` to the HTML file.
3. Observe the element's width.  The incorrect code will likely render incorrectly, while the correct code will render as expected.