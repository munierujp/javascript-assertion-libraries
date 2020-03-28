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
