# SVG namespacing

Default svg export of Sketch 3.8 has a problem when inlining many svgs in one html.
There are many ids with **very general name** such as `path-1`, `path-2`, etc. If many inline svgs exported from Sketch 3.8 are in one HTML file, the first id would override following same ids.

This plugin do BEM-style namespacing. If you export a slice named `Button`, all ids in exported svg are converted like `Button--path-1`.

Currently it only namespaces slices, just because this way fits our requirement.

This plugin requires Sketch 3.8.

# Install

1. [Go to releases page](https://github.com/Knowre-Dev/svg-namespacing/releases/latest) and download `Source code (zip)` file.
1. Extract it in any folder.
1. Double click `SVG namespaceing.sketchplugin` in finder.
1. Done! From now on, all svg files exported from slices are namespaced.
