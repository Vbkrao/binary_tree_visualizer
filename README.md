# Binary Tree Visualization

This project visualizes binary trees using HTML5 Canvas. It provides a utility to draw and connect nodes dynamically based on user input.

## Key Concepts

- **Tree Characteristics:** Represents binary trees where each node has at most two children. The height of the tree and node positions are crucial for visualization.

- **Coordinate System:** Utilizes a canvas coordinate system to position nodes. Nodes are spaced horizontally and vertically based on their depth and width.

- **Real-Time Coordinates:** Calculates node positions dynamically to fit the canvas size and tree structure. Adjusts node rendering to ensure correct placement and spacing.

- **Bezier Curves:** Used to draw smooth curves between nodes. The curve is defined by control points to connect parent and child nodes visually.

- **Convex Hull:** Although not explicitly used in this project, convex hulls can define boundaries around groups of nodes in advanced visualizations.

- **Parsing User Data:** Parses and constructs a binary tree from user input. Cleans and splits input data, then builds the tree using a level-order traversal.

## Files

- `BinaryTreeNode.js`: Defines the binary tree node structure.
- `treeUtils.js`: Contains utility functions for calculating dimensions, drawing nodes, connecting edges, and constructing the tree.
- `index.html`: Provides the user interface for input and rendering.
- `drawBinaryTree.js`: Implements the drawing logic and handles user interactions.

## Usage

1. **Input Tree Data:** Enter a comma-separated list of node values into the textarea.
2. **Render Tree:** Click "Apply" to visualize the tree. The canvas will update to show the tree structure.
3. **Clear Canvas:** Click "Clear" to reset the input and canvas.


