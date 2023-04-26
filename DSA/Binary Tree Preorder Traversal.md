
https://leetcode.com/problems/binary-tree-preorder-traversal/solutions/2918429/binary-tree-preorder-traversal/

```typescript
function preorderTraversal(root: TreeNode | null): number[] {
	// 1) First check if empty
    if (!root) return [];
    const result = []
    // 2) Add first element to the stack so we can 
    // iterate over
    const stack = [root];

    while (stack.length) {
	    // 3) First iteration we take the first off the stack
	    // and then push its value into the result
        const node = stack.pop();
        result.push(node.val);

		// 4) We check LHS && RHS and add them to the stack
		// we add RHS first because when we pop off in the next 
		// ite
		// add the LHS value first and we will then come back
		// to the RHS
        if (node.right) {
            stack.push(node.right);
        }

        if (node.left) {
            stack.push(node.left);
        }

		// 5) We then repeat this in that order
    }

    return result;
}
```

![[Pasted image 20230102213531.png]]

So if we take the above example we would go in the following order with our stack:

The result for the above would be: ` 5, 4, 2, 3, 6, 8 `

Our stack order would go as follows:
`5`
`6, 4`
`6, 3, 2`
`6, 3`
`6`
`8`


