# jest-dify-snapshot

[![npm version](https://img.shields.io/npm/v/jest-dify-snapshot.svg)](https://www.npmjs.com/package/jest-dify-snapshot)
[![npm downloads](https://img.shields.io/npm/dm/jest-dify-snapshot.svg)](https://www.npmjs.com/package/jest-dify-snapshot)

## Usage

### 1. Install

```sh
npm i --save-dev jest-dify-snapshot
# or if you are using yarn
yarn --save-dev jest-dify-snapshot
```

### 2. Extend Jest expect

```js
const { toMatchImageSnapshot } = require('jest-dify-snapshot');
expect.extend({ toMatchImageSnapshot });
```

### 3. Use `expect(...).toMatchImageSnapshot()`

```js
it('should match image snapshot', () => {
  // ...
  expect(img).toMatchImageSnapshot();
});
```
