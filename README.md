# Hello WASM

## Description
A simple hello wasm package that allows you to add in javascript
using web assembly. This helps with speed boots and other things.

## Run
```bash
wasm-pack build --target web
```
```bash
python3 -m http.server
```

## Example
```js
import init, { add } from './pkg/hello_wasm.js';

await init();
console.log(add(1, 2));
```
