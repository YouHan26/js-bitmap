# js-bitmap

# Install
```js
yarn add js-bitmap
```

# Usage
```js
import BitMap from 'js-bitmap';

function test() {
  const bitmap = new BitMap();
  for (let i = 0; i < 10000;) {
    bitmap.push(i);
    i += Math.floor(Math.random() * 5 + 10);
  }
  for (let i = 0; i < 10000; i++) {
    if (bitmap.isExist(i)) {
      console.log(i);
    }
  }
}

test();

```

# API
* push(n: Number)
* isExist(n: Number) 
* clear()