# Hello WASM

## Description
A simple hello wasm package that allows you to add in javascript
using web assembly. This helps with speed boots and other things.

## Install dependencies
wasm-pack: https://rustwasm.github.io/wasm-pack/installer/
```bash
curl https://rustwasm.github.io/wasm-pack/installer/init.sh -sSf | sh
```

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
