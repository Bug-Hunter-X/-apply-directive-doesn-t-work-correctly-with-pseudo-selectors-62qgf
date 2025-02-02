# Tailwind CSS @apply Directive Issue with Pseudo-Selectors

This repository demonstrates a bug encountered when using Tailwind CSS's `@apply` directive with pseudo-selectors such as `:hover`, `:focus`, and `:active`. The issue arises when the `@apply` directive is used within a pseudo-selector class; the styles are not applied correctly to the child elements.

## Bug Description

The `@apply` directive, when placed within a pseudo-selector class (e.g., `:hover`), fails to cascade the styles to the child elements as expected. This can lead to unexpected behavior where hover effects, focus styles, or active states don't function correctly.

## Solution

The solution is to avoid using `@apply` within pseudo-selector classes. Instead, directly apply the individual Tailwind CSS utility classes to the element and its pseudo-selectors. Alternatively, use a different approach for handling styles based on the element's state.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the hover effect does not work as expected.
4. Open `bugSolution.html` to see the corrected implementation.
