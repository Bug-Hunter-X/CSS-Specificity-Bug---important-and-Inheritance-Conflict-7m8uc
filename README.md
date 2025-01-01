# CSS Specificity Bug: !important and Inheritance Conflict

This repository demonstrates an uncommon bug in CSS related to the interaction of `!important`, inheritance, and specificity.

## The Bug
The provided CSS code snippet showcases an unexpected behavior where `!important` doesn't fully override an inherited style.  The `p` element inherits a `font-size` from its parent, and even with `!important`, the inherited style persists.

## Solution
The solution involves understanding the order of operations.  The inheritance happens before the `!important` rule is applied.  Therefore, the solution might require more explicit styling or applying the `!important` to both the parent and the child element if the inheritance needs to be totally overridden.