### Buffer in JavaScript
1. Buffer exist in Node.Js, but not in browser. Webpack provides [shim](https://webpack.js.org/configuration/node/) for it. 

2. Data is JavaScript can be stored in data array: e.g. ```Uint8Array```.

4. ```GetObject``` API from ```s3``` returns data in such format, sometimes.

3. To create a data array:
    ```js
    const array = Uint8Array.from([1, 2, 3]);
    ```
4. To creat a buffer:
    ```js
    const ab = Buffer.from(array);
    ```
5. ArrayBuffer back to array: 
    ```js
    [...buffer]
    ```
