# javascript-assertion-libraries
## Libraries
- [Node.js](https://nodejs.org/api/assert.html)
- [Chai](https://www.chaijs.com/)
  - [Assert](https://www.chaijs.com/guide/styles/#assert)

## Base
### `value` is truthy
- Node.js

```js
assert.ok(value)
```

```js
assert(value)
```

- Chai

```js
assert.isOk(value)
```

### `value` is falsy
- Node.js

```js
assert.ok(!value)
```

```js
assert(!value)
```

- Chai

```js
assert.isNotOk(value)
```

## Equality
### `actual` is strictly equal to `expected`
- Node.js

```js
assert.strictEqual(actual, expected)
```

- Chai

```js
assert.strictEqual(actual, expected)
```

### `actual` is not strictly equal to `expected`
- Node.js

```js
assert.notStrictEqual(actual, expected)
```

- Chai

```js
assert.notStrictEqual(actual, expected)
```

### `actual` is deeply and strictly equal to `expected` 
- Node.js

```js
assert.deepStrictEqual(actual, expected)
```

- Chai

none

### `actual` is not deeply and strictly equal to `expected` 
- Node.js

```js
assert.notDeepStrictEqual(actual, expected)
```

- Chai

none

## nullish
### `value` is `null`
- Node.js

```js
assert.strictEqual(value, null)
```

- Chai

```js
assert.isNull(value)
```

### `value` is  not `null`
- Node.js

```js
assert.notStrictEqual(value, null)
```

- Chai

```js
assert.isNotNull(value)
```

### `value` is `undefined`
- Node.js

```js
assert.strictEqual(value, undefined)
```

- Chai

```js
assert.isUndefined(value)
```

### `value` is  not `undefined`
- Node.js

```js
assert.notStrictEqual(value, undefined)
```

- Chai

```js
assert.isDefined(value)
```

### `value` is `null` or `undefined`
- Node.js

```js
assert(value == null)
```

```js
assert(value == undefined)
```

- Chai

```js
assert.notExists(value)
```

### `value` is not `null` or `undefined`
- Node.js

```js
assert(value != null)
```

```js
assert(value != undefined)
```

- Chai

```js
assert.exists(value)
```
