# Voxel Sparrow - 3D Strip Packing in Python

## Demo / Portfolio Showcase

Voxel Sparrow is a Python research prototype for packing irregular voxel objects into a strip with fixed width and depth while reducing its height.

This page presents the project's capabilities and a recorded demonstration. It is a visual showcase, not a downloadable software release or a hosted interactive application. The implementation is not distributed through this page.

## Demonstration

![Recorded demonstration of voxel-based packing compression](results/chess_1000/packing.gif)

The animation illustrates the packing search and changes in strip height. It is a demonstration of one run, not a performance comparison or a guarantee of optimality.

## Capabilities

| Capability | Description |
| --- | --- |
| Irregular 3D packing | Packs voxel objects within a fixed-width, fixed-depth strip while searching for a lower packing height. |
| Orientation search | Considers up to 24 proper orthogonal orientations when rotation is enabled. |
| Clearance constraints | Supports configurable spacing between objects and between objects and container boundaries. |
| Adaptive compression | Adjusts compression steps according to search progress within a configurable computational budget. |
| Interactive inspection | The private implementation includes a 3D viewer for inspecting layouts and results. |
| Search visualisation | Produces compression animations and search traces for reviewing optimisation progress. |
| Experimental workflows | Includes batch processing, result summaries, geometric auditing, and automated checks. |

## Technical Highlights

- Python and NumPy for voxel-based geometric computation and heuristic search.
- Structured configuration and solution outputs for computational experiments.
- Modular source organisation, Git version control, usage documentation, and automated checks.
- Visualisation tools connecting optimisation results with interpretable 3D layouts.

These features describe the underlying implementation. Source code, installation instructions, execution scripts, and datasets are not provided as part of this showcase.

## Method and Limitations

This prototype is a heuristic voxel adaptation of Sparrow. It is not an exact reproduction of the original method and does not guarantee an optimal solution. Geometric checks apply to the voxel representation and its configured clearance rules. Search outcomes can depend on the time budget and run conditions.

## Original Sparrow and Research Reference

This prototype adapts ideas from **Sparrow**, the 2D irregular strip-packing heuristic developed by Jeroen Gardeyn and collaborators, to a 3D voxel-based setting in Python. Credit for the original Sparrow method belongs to its authors. This prototype is not an exact reproduction of their algorithm, and the original paper's performance results do not describe this implementation.

- **Original repository:** [JeroenGar/sparrow](https://github.com/JeroenGar/sparrow).
- **Paper:** Jeroen Gardeyn, Greet Vanden Berghe, and Tony Wauters. *An open-source heuristic to reboot 2D nesting research*. arXiv:2509.13329, first submitted in 2025. [Read the paper](https://arxiv.org/abs/2509.13329) · [DOI](https://doi.org/10.48550/arXiv.2509.13329).

Please consult the original repository and paper for the original 2D method and its evaluation.

## Availability and Permissions

This page is provided for portfolio and demonstration purposes. It does not offer the underlying implementation or datasets under an open-source licence. Any reuse of demonstration materials beyond permissions already applicable requires permission from the relevant rights holder.

