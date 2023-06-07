```javascript

// Given an integer array `nums` and an integer `k`, return _the_ `k` _most frequent elements_. You may return the answer in **any order**.

const topKFrequent = function(nums, k) {
    const count = new Map();
    const freq = new Array(nums.length + 1); // 1) Create a bucket that matches length of nums + 1

    for (let i = 0; i < nums.length; i++) {
        if (count.has(nums[i])) {
            count.set(nums[i], count.get(nums[i]) + 1);
        } else {
            count.set(nums[i], 1);
        }
    } // 2) Populate the amount of times each number appears in a Map

    for (let [k, c] of count) {
        if (freq[c]) {
            freq[c].push(k);
        } else {
            freq[c] = [k];
        }
    } // 3) Loop over the map and use the count value as the index for the bucket and then use the key for the value. This is an array of arrays in case there are more than one 

    const result = [];

    for (let i = freq.length; i > 0; i--) {
        if (result.length === k) {
            return result;
        }

        if (freq[i]) {
            result.push(...freq[i]);
        }
    } // 4) Loop over the freq and then create a result. Each time checking if you reached your target length result. Since it is an array of arrays destructure each.

    return result;
};

console.log(topKFrequent([1, 1, 1, 2, 2, 3], 2));
console.log(topKFrequent([1], 1));
```

