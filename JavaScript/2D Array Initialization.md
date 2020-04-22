### 2D Array Initialization
To initialize a ```m * n``` 2d array of in modern JavaScript:
```js
[...Array(m)].map(e => Array(n));
```

Notes:

```Array(m).map(e => Array(n))``` doesn't work, because Array(m) generates ```[ <m empty items> ]```.
That's not iterable. 
But apparently, ```[...Array(m)]``` will turn empty items into ```undefined```, which is iterable.
