
## Gold Find Problem

```js
function getMaximumGold(grid) {
    let max = 0;
    const rowCount = grid.length;
    const colCount = grid[0].length;

    for (let r = 0; r < rowCount; r++) {
        for (let c = 0; c < colCount; c++) {
            let sum = findGold(0, grid, rowCount, colCount, r, c);
        }
    } 
    
    function findGold(sum, grid, rowCount, colCount, r, c) {
        if (r < 0 || c < 0 || r === rowCount || c === colCount || grid[r][c] === 0) {
	        return;
        }

        const value = grid[r][c];
        const temp = value;
        grid[r][c] = 0;
        sum += value;
        
        findGold(sum, grid, rowCount, colCount, r, c + 1);
        findGold(sum, grid, rowCount, colCount, r, c - 1);
        findGold(sum, grid, rowCount, colCount, r + 1, c);
        findGold(sum, grid, rowCount, colCount, r - 1, c);

        max = Math.max(sum, max);
        grid[r][c] = temp;
    }

    return max;
};
```