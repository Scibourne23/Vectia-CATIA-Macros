# Vectia Tools for CATIA V5

Vectia is an engineering productivity platform for CATIA V5. This toolkit of powerful macros streamlines critical workflows from initial design to final documentation. It's built to accelerate development, reduce manual error, and empower the modern engineer.

---

## Features

*   **Intelligent Automation:** Scripts are designed with context-aware logic to handle complex scenarios and reduce user prompts.
*   **Workbench Agnostic:** Provides powerful enhancements across Part Design, Assembly Design, and Drafting workbenches.
*   **User-Friendly:** Built with clear instructions, user-configurable options, and a focus on stable, predictable results.
*   **Production-Ready:** Developed and tested to solve real-world challenges in a demanding automotive design environment.

---

## Macro Suite

The suite is organized by the primary CATIA V5 workbench where the tool is used.

### Drafting & 2D Annotation

#### 1. Master Text Numbering (`DimNumberingCompStd_v2.txt`)
The flagship macro for creating visually perfect, associative VVNN numbering. It uses a pre-selected text object as a template, ensuring perfect compliance with any custom graphical standard (including custom frames/oblongs).
*   **How to Use:** Select your "Master Text" object first, then CTRL+select all target Dimensions/GDTs. Run the macro and follow the prompts.

#### 2. Smart Bault/Upper Text Numbering (`DimNumberingReset.txt`)
An intelligent tool for editing existing drawings. It scans views for the highest existing VVNN number and continues the sequence by modifying the `BaultText` of dimensions or the `Upper Text` of GDTs.
*   **How to Use:** Select all target Dimensions and GDTs you wish to number. Run the macro and follow the prompts.

#### 3. Drawing Reset Utility (`ResetDrawingUtility2D.txt`)
A powerful cleanup tool for removing specific annotations from a drawing sheet or a single view.
*   **How to Use:** Run the macro and choose from the menu whether to delete VVNN numbering text, revision balloons, or both, and from which scope (active view or all views).

#### 4. Sequential Text Editor (`TextSequenceEdit2D_v1.txt`)
A simple utility for quickly renumbering a series of selected text objects.
*   **How to Use:** Select a series of `DrawingText` objects in the desired order. Run the macro and provide a prefix (optional) and a starting number.

---

### Part Design & 3D Geometry

#### 1. Bounding Box Wireframe Creator (`MakeBoundingBox3D_v1.txt`)
Creates a complete, accurate wireframe bounding box around a selected Body or HybridBody, aligned to a chosen axis system. The macro creates all necessary construction geometry and places the final result in a clean "Bounding_Box_Wireframe" geometrical set.
*   **How to Use:** Run the macro and follow the prompts to select the target body and the reference axis system.

#### 2. Extremum Points Creator (`MakeExtremums.txt`)
A focused utility that generates the 6 extremum points (Min/Max for X, Y, Z) for a selected body relative to a reference axis system.
*   **How to Use:** Run the macro and follow the prompts to select the target body and the reference axis system.

#### 3. Smart Feature Renamer (`SmartRenamingPtsandSurfs_v1.txt`)
A versatile tool for sequentially renaming any selected features in the specification tree (Points, Surfaces, Planes, etc.). It intelligently handles leading zeros based on the user's starting number.
*   **How to Use:** Select the features you want to rename in the desired order. Run the macro and provide a prefix (optional) and a starting number (e.g., `1`, `01`, `001`).

---

### Assembly Design

#### 1. Simple 3D Explode Scene (`ExplodeScene3D_v1.txt`)
Creates a simple, linear exploded view by moving selected parts along a global axis. This macro directly modifies part positions and is best used within the "Enhanced Scene" workbench to avoid overriding assembly constraints.
*   **How to Use:** Select all parts to be exploded in the specification tree. Run the macro and provide the explosion axis (X, Y, or Z) and the spacing distance.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments
This project was created by [**Your Name / Your GitHub Username**], a Mechanical Design Engineer at Visteon, in collaboration with an advanced AI assistant specializing in CATIA V5 automation.
