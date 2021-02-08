### [Nullish coalescing](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Nullish_coalescing_operator)

I used to write something like ```(map.get('abc') || 1)``` to set a default value as `1`, only in case the key `abc` does not exist.

But that has an unintended behavior: If the value of the map is allowed to be `0`, which is `falsy`, the right hand side of `||` still excutes.

Now nullish coalescing `??` only executes right hand side iff the left hand side is `null` or `undefined`. It perfect solves the problem.


### [Optional chaining](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining)

Just use it in place of `lodash.get`! Great!
`const petName = person.pet?.name`
