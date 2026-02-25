# 3DsMaxCleanPivot
Purpose:
This 3ds Max 2024 script creates clean duplicates of selected objects while preserving their original hierarchy, transferring animation and modifiers from the originals. It’s designed to safely reset object transformations (Reset XForm) and convert them to Editable Poly without losing key data.

Features:

Clean Copies:

-Creates duplicates of the selected objects.

-Removes all animation and modifiers initially to ensure a clean base.

-Applies Reset XForm and converts each object to Editable Poly.

-Restores the original transform (position, rotation, scale) after Reset XForm.


Hierarchy Restoration:

-Rebuilds the original parent-child relationships for all copied objects.

-Supports multiple levels of nested hierarchy.


Animation Transfer:

-Copies position, rotation (Euler XYZ), and scale animation controllers from the original objects to their duplicates.

-Works for objects with or without existing animation.


Modifiers Transfer:

-Copies all modifiers from the original objects to the duplicates.

-Ensures that the duplicates maintain the same modifier stack as the originals.


Usage:

-Select one or more objects in the scene.

-Run the script.

-The script will create "_clean" duplicates of the selected objects in active layer.

-At the end, the duplicates will have:

-Reset transforms with Editable Poly applied

-Original hierarchy restored

-Animation and modifiers copied from the original objects


Notes:
-Works with Editable_Mesh and Editable_Poly objects.

-Maintains animation and modifiers safely even after Reset XForm.

-Ideal for preparing clean rigs or models for export, batching, or further editing, for transfer to Blender via fbx files.
