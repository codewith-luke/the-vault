## Stack with Recursive Backtrack

```js
var generateParenthesis = function(n) {
    
    let stack = [];
    let result = [];

    function backtrack(open, close){
        if(open == close && open == n) {
            result.push(stack.join(''));
            return;
        }

        if(open < n){
            stack.push('(');
            backtrack(open+1, close);
            stack.pop()
        }
        if(close < open){
            stack.push(')');
            backtrack(open, close+1);
            stack.pop();
        }

    }
    backtrack(0,0)
    return result
};
```

The above when given an a count of 2 will follow the following stack:

```
(
((
(())
(()
(
()(
()()
()(
()
(
```

This happens as it will first go forward on the route of `(())` for any count amount and then it will try all the variations of that until it would reach where all brackets match `()()`