# Palindrome
```javascript
var isPalindrome = function(s) {
    let newStr = s.toLowerCase().replace(/[^0-9a-z]/g, "");
    let left = 0, right = newStr.length-1;
    
    while(left < right){
        if(newStr[left] !== newStr[right]) return false
        left++
        right--
    }
    return true
};
```

# Two Sum Two Pointer

```js
const twoSum = function (arr, target) {
    let lhs = 0;
    let rhs = arr.length - 1;

    while (lhs < rhs) {
        let sum = arr[lhs] + arr[rhs];
        
        if (sum === target) {
            lhs++;
            rhs++;
            return [lhs, rhs];
        }
        
        if (sum > target) {
            rhs--;
        } else {
            lhs++;
        }
    }
};
```

# 3 Sum

```js
function threeSum(nums) {
    const res = []; // Initialize the result array
    nums.sort((a, b) => a - b); // Sort the input array in ascending order

    for (let i = 0; i < nums.length; i++) {
        // Iterate through the array elements
        if (nums[i] > 0) {
            // If the current element is positive, break the loop
            break;
        }

        if (i > 0 && nums[i] === nums[i - 1]) {
            // Skip duplicate elements to avoid duplicate triplets
            continue;
        }

        let l = i + 1; // Pointer for the left element
        let r = nums.length - 1; // Pointer for the right element

        while (l < r) {
            // Loop through the subarray
            const threeSum = nums[i] + nums[l] + nums[r]; // Calculate the sum of three elements

            if (threeSum > 0) {
                // If the sum is greater than 0, decrease the right pointer
                r--;
            } else if (threeSum < 0) {
                // If the sum is less than 0, increase the left pointer
                l++;
            } else {
                // If the sum is equal to 0, it is a valid triplet
                res.push([nums[i], nums[l], nums[r]]); // Add the triplet to the result array
                l++;
                r--;

                while (nums[l] === nums[l - 1] && l < r) {
                    // Skip duplicate elements to avoid duplicate triplets
                    l++;
                }
            }
        }
    }

    return res; // Return the final result array
}
```