# CSS Specificity Bug

This repository demonstrates a common issue in CSS related to selector specificity.  The inner div with class 'special' unexpectedly inherits a different style than intended due to the way CSS resolves conflicting styles.

## Problem

The problem lies in how CSS handles cascading stylesheets when multiple selectors target the same element. The selector `.container .special` has higher specificity than `.container div.special`, resulting in the unexpected override.

## Solution

To fix this, refactor the CSS to ensure the intended style is applied based on the required specificity.  The solution provides a modified CSS file that resolves the issue by applying the correct styling through improved selector specificity or using the `!important` flag cautiously.