# Binary Tree Visualization

This project provides a utility for visualizing binary trees using HTML5 Canvas. The code includes a basic binary tree implementation and functions to draw and connect nodes on a canvas.

## Project Structure

### `BinaryTreeNode.js`

Defines the `BinaryTreeNode` class used for representing nodes in a binary tree.

```javascript
export class BinaryTreeNode {
    value = null;
    left = null;
    right = null;

    constructor(value) {
        this.value = value;
        this.left = null;
        this.right = null;
    }

    setLeft(node) {
        this.left = node;
    }

    setRight(node) {
        this.right = node;
    }

    getHeight() {
        const leftHeight = this.left?.getHeight() || 0;
        const rightHeight = this.right?.getHeight() || 0;

        return Math.max(leftHeight, rightHeight) + 1;
    }
}
