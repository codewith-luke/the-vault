## Largest Substring

```js
const lengthOfLongestSubstring = function(s) {
    if (s.length <= 1) return s.length;

    let subSet = new Set();
    let left = 0;
    let max = 0;

    for (let i = 0; i < s.length; i++) {
	    // NOTE: Here we have to keep shifting 
	    // until we have remove all possible duplicates.
        while (subSet.has(s[i])) {
            subSet.delete(s[left]);
            left++;
        }
        
        subSet.add(s[i]);
        max = Math.max(max, i - left + 1);
    }

    return max;
};
```

## Longest Repeating Character Replacement

```js
var characterReplacement = function (s, k) {
    let [left, right, longest, max] = new Array(4).fill(0);
    const frequencyMap = new Array(26).fill(0);

    while (right < s.length) {
        const count = addRightFrequency(s, right, frequencyMap);

        longest = Math.max(longest, count);

        let window = right - left + 1;
        const canSlide = k < window - longest;


        if (canSlide) {
            subtractLeftFrequency(s, left, frequencyMap);
            left++;
        }
        
        window = right - left + 1;
        max = Math.max(max, window);

        right++;
    }

    return max;
};

const addRightFrequency = (s, right, map) => {
    const char = s[right];
    const index = getCode(char);

    map[index]++;

    return map[index];
};

const subtractLeftFrequency = (s, left, map) => {
    const char = s[left];
    const index = getCode(char);

    map[index]--;

    return map[index];
};

const getCode = (char) => char.charCodeAt(0) - 'A'.charCodeAt(0);
```

```
"ABAB" 1
Result: 3 as we can replace BAB => AAA longest window would then be 3
```