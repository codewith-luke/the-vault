# Basic

```js
function binarySearch(arr, target) {
  let left = 0;
  let right = arr.length - 1;

  while (left <= right) {
    const mid = Math.floor((left + right) / 2);

    if (arr[mid] === target) {
      return mid; // Target found, return its index
    } else if (arr[mid] < target) {
      left = mid + 1; // Target is in the right half of the array
    } else {
      right = mid - 1; // Target is in the left half of the array
    }
  }

  return -1; // Target not found
}

// Example usage:
const numbers = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20];
const targetNumber = 12;

console.log(binarySearch(numbers, targetNumber));
```

## 2D Matrix (Nested Binary)

```js
const searchMatrix = function (matrix, target) {
    let ml = 0;
    let mr = matrix.length - 1;

    while (ml <= mr) {
        const matrixMid = Math.floor((ml + mr) / 2);
        const row = matrix[matrixMid];
        let l = 0;
        let r = matrix[matrixMid].length - 1;

        while (l <= r) {
            const mid = Math.floor((l + r) / 2);
            if (row[mid] === target) return true

            if (row[mid] < target) {
                l = mid + 1;
            } else {
                r = mid - 1;
            }
        }

        l = 0;
        r = 0;
        if (matrix[matrixMid][0] < target) {
            ml = matrixMid + 1
        } else {
            mr = matrixMid - 1
        }
    }

    return false;
};

console.log(searchMatrix([[1, 3, 5, 7], [10, 11, 16, 20], [23, 30, 34, 60]], 3));
console.log(searchMatrix([[1], [3]], 3));
```

# Imaginary Array Binary Search

The idea here being that you are using the unsorted array to determine your range and using the h as your target that you want to be within.

```js
function minEatingSpeed(piles, h) {
    let k = Infinity;
    let left = 1;
    let right = Math.max(...piles);
    let mid = Math.floor((left + right) / 2);

    while (left <= right) {
        let sum = 0;

        for (let i = 0; i < piles.length; i++) {
            sum = sum + Math.ceil(piles[i] / mid);
        }

        if (sum <= h) {
            k = Math.min(k, mid);
            right = mid - 1;
            mid = Math.floor((left + right) / 2);
        } else {
            left = mid + 1;
            mid = Math.floor((left + right) / 2);
        }
    }

    return k;
}

console.log(minEatingSpeed([3, 6, 11, 7], 8)) // 4
```

# Binary Shifted Search

```js
var search = function (nums, target) {
    let left = 0;
    let right = nums.length - 1;

    while (left <= right) {
        let mid = Math.floor((left + right) / 2);

        if (target === nums[mid]) {
            return mid;
        }

        if (nums[left] <= nums[mid]) {
            if (nums[left] <= target && nums[mid] >= target) {
                right = mid - 1;
            } else {
                left = mid + 1;
            }
        } else {
            if (nums[right] >= target && nums[mid] <= target) {
                left = mid + 1;
            } else {
                right = mid - 1;
            }
        }
    }
    return -1;
}

console.log(search([4, 5, 6, 7, 0, 1, 2], 0)); // 4
console.log(search([4, 5, 6, 7, 0, 1, 2], 6)); // 2

```