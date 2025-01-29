# CSS calc() Calculation Errors

This repository demonstrates a common issue encountered when using the `calc()` function in CSS: incorrect calculations due to unresolved dimensions of the parent element. The `calc()` function performs calculations directly within your CSS. However, if the dimensions it relies on (e.g. parent's width) are not yet determined when the calculation is evaluated, `calc()` might yield unexpected values, commonly 0.

The example `bug.css` shows this issue, resulting in an element that initially appears incorrectly sized. The solution (`bugSolution.css`) provides a possible fix using a JavaScript workaround or altering the CSS structure to avoid the circular dependency.