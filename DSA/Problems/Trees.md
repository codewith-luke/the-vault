# Invert Binary Tree

## Recursion

```js 
const invertTree = function(root) {
 if (!root) return root;  
  
  const tmp = root.left;
  root.left = root.right;
  root.right = tmp;

  invertTree(root.left);
  invertTree(root.right);

  return root;
};
```

## While Loop with Queue

```js
const invertTree = function (root) {
    if (!root) return root;

    const q = [];

    q.push(root);

    while (q.length > 0) {
        let cur = q.shift();
        let left = cur.left;
        let right = cur.right;

        cur.left = right;
        cur.right = left;

        if (cur.left) {
            q.push(cur.left);
        }

        if (cur.right) {
            q.push(cur.right);
        }
    }
    return root;
}
```

# Max Depth

## Recursion
```js
const maxDepth = function(root) {
    if(root == null)  return 0;

    let leftDepth = maxDepth(root.left);
    let rightDepth = maxDepth(root.right);
    return Math.max(leftDepth, rightDepth) + 1;
};
```

## While using tracking of current depth
```js
function maxDepth(root) {
    let maximumDepth = 0;
    const nodesToTraverse = [[root, 1]];

    while(nodesToTraverse.length) {
        const [node, depth] = nodesToTraverse.pop();

        if(!node) {
            continue;
        }

        maximumDepth = Math.max(maximumDepth, depth);
        nodesToTraverse.push([node.left, depth + 1]);
        nodesToTraverse.push([node.right, depth + 1]);
    }

    return maximumDepth;
}
```

## While Iterative

```js
const maxDepth = (root) => {
    if (!root) return 0;
    const queue = [root];
    let depth = 0;
    while (queue.length !== 0) {
        const len = queue.length;
        
        for (let i = 0; i < len; i++) {
            let item = queue.shift()
            if (item.left) queue.push(item.left);
            if (item.right) queue.push(item.right);
        }
        
        depth++;        
    }
    
    return depth;
};
```

# Diameter

```js
const diameterOfBinaryTree = (root) => {
    if (!root) return 0

    let maxDiameter = 0

    const dfs = (node) => {
        if (!node) return 0

        let left = dfs(node.left)
        let right = dfs(node.right)

        maxDiameter = Math.max(maxDiameter, left + right)

        return Math.max(left, right) + 1
    }

    dfs(root)
 
    return maxDiameter
};
```

# Balanced Height

```js
const isBalanced = function(root) {
    let flag = true;
    
    var height = function(r){
        if(!r) return 0;
    
        let num1 = height(r.left);
        let num2 = height(r.right);
        let res = num1 - num2;
    
        if(res < -1 || res > 1) flag = false;
    
        return Math.max(num1,num2) + 1;
    }
    
    height(root);
    return flag;
};
```

# Compare 2 Trees

## Recursive

```js
const isSameTree = function(p, q) {
    if (!p && !q) return true; // Check if both trees are empty
    if (!p || !q) return false; // Check if either tree is empty

    const dfs = (nodeA, nodeB) => {
        if (!nodeA && !nodeB) return true; // Both nodes are empty
        if (!nodeA || !nodeB) return false; // Either node is empty
        if (nodeA.val !== nodeB.val) return false; // Values are not equal

        // Recursively check the left and right subtrees
        return dfs(nodeA.left, nodeB.left) && dfs(nodeA.right, nodeB.right);
    };

    return dfs(p, q);
};
```

## Iterative

```js
function isSameTree(p, q) {
    let curr = p;
    let opp = q;
    const stack = [];
    const oppStack = [];

    if(!curr && !opp) return true

    do {
        if(curr?.val !== opp?.val) return false;
        
        if (curr) {
            stack.push(curr);
            oppStack.push(opp);
            curr = curr.left;
            opp = opp.left;
        } else {
            curr = stack.pop();
            opp = oppStack.pop();
            curr = curr.right;
            opp = opp.right;
        }
    }
    while (stack.length || oppStack.length || curr || opp);

    return true
};
```

# Contains Subtree

```js
const isSubtree = (root, subRoot) => {
  const areEqual = (node1, node2) => {
    if (!node1 || !node2) return !node1 && !node2;
    if (node1.val !== node2.val) return false;
    return areEqual(node1.left, node2.left) && areEqual(node1.right, node2.right);
  }
  const dfs = (node) => {
    if (!node) return false;
    if (areEqual(node, subRoot)) return true;
    return dfs(node.left) || dfs(node.right);
  }
  return dfs(root);
};
```

# Validate BST

```js
const isValidBST = function(root) {
    let valid = true;

    function wrap(node, min, max) {
        if (!node) return;
        
        if(!(node.val > min) || !(node.val < max)) {
            valid = false;
            return;
        };
        
    
        wrap(node.left, min, node.val);
        wrap(node.right, node.val, max);
    }

    wrap(root, -Infinity, Infinity);

    return valid;
};
```