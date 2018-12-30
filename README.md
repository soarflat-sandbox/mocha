# mocha

Mocha と戯れる。

## INSTALLATION

```bash
$ npm install --save-dev mocha
```

## GETTING STARTED

```bash
$ mkdir test
$ touch test/test.js # open with your favorite editor
```

**test/test.js**

```js
const assert = require('assert');
describe('Array', () => {
  describe('#indexOf()', () => {
    it('should return -1 when the value is not present', () => {
      assert.equal([1, 2, 3].indexOf(4), -1);
    });
  });
});
```

ターミナルでテスト実行。

```bash
$ mocha

  #以下が出力される
  Array
    #indexOf()
      ✓ should return -1 when the value is not present

  1 passing (5ms)
```
