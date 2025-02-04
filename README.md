# TailwindCSS @apply in @layer: Unexpected Behavior with Cross-Layer Styles

This repository demonstrates a bug encountered when using Tailwind's `@apply` directive within a `@layer` directive. The issue occurs when the `@apply` directive attempts to apply styles defined in a different layer.

## Bug Description
The `@apply` directive does not correctly apply styles defined in other layers, leading to unexpected results in the final rendered output.  This behavior is inconsistent with expectations and makes using layers with `@apply` difficult.

## Reproduction
1. Clone this repository.
2. Compile the CSS using your preferred TailwindCSS build process.
3. Observe the rendered output. The styles applied using `@apply` from a different layer will either not be applied or will be applied incorrectly, showcasing the issue.

## Solution
The solution involves refactoring the CSS structure to ensure that `@apply` is used within the same layer as the classes being applied.  This ensures consistency and predictable behavior.

## Contributing
Contributions are welcome! If you have a solution or a better understanding of this issue, feel free to open a pull request.