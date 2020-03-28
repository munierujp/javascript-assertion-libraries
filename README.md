# JavaScript Assertion Libraries
## Libraries
- [Node.js](https://nodejs.org/api/assert.html)
- [Chai](https://www.chaijs.com/)
  - [Assert](https://www.chaijs.com/guide/styles/#assert)
- [Jest](https://jestjs.io/)

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

- Jest

```js
expect(value).toBeTruthy()
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

- Jest

```js
expect(value).toBeFalsy()
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

- Jest

```js
expect(actual === expected).toBe(true)
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

- Jest

```js
expect(actual !== expected).toBe(true)
```

### `actual` is deeply and strictly equal to `expected` 
- Node.js

```js
assert.deepStrictEqual(actual, expected)
```

- Chai

none

- Jest

none

### `actual` is not deeply and strictly equal to `expected` 
- Node.js

```js
assert.notDeepStrictEqual(actual, expected)
```

- Chai

none

- Jest

none

### `actual` is same value to `expected`
- Node.js

```js
assert(Object.is(value, expected))
```

- Chai

```js
assert.isOk(Object.is(value, expected))
```

- Jest

```js
expect(value).toBe(expected)
```

### `actual` is not same value to `expected`
- Node.js

```js
assert(!Object.is(value, expected))
```

- Chai

```js
assert.isNotOk(Object.is(value, expected))
```

- Jest

```js
expect(value).not.toBe(expected)
```

### `actual` is deeply same value to `expected`
- Node.js

none

- Chai

none

- Jest

```js
expect(value).toEqual(expected)
```

### `actual` is not deeply same value to `expected`
- Node.js

none

- Chai

none

- Jest

```js
expect(value).not.toEqual(expected)
```

## Existence
### `value` is `null`
- Node.js

```js
assert.strictEqual(value, null)
```

- Chai

```js
assert.isNull(value)
```

- Jest

```js
expect(value).toBeNull()
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

- Jest

```js
expect(value).toBeUndefined()
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

- Jest

```js
expect(value).toBeDefined()
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

## object
### `value` is plain object
- Node.js

none

- Chai

```js
assert.isObject(value)
```

### `value` is not plain object
- Node.js

none

- Chai

```js
assert.isNotObject(value)
```

## boolean
### `value` is boolean
- Node.js

```js
assert.strictEqual(typeof value, 'boolean')
```

- Chai

```js
assert.isBoolean(value)
```

### `value` is not boolean
- Node.js

```js
assert.notStrictEqual(typeof value, 'boolean')
```

- Chai

```js
assert.isNotBoolean(value)
```

### `value` is `true`
- Node.js

```js
assert.strictEqual(value, true)
```

- Chai

```js
assert.isTrue(value)
```

### `value` is not `true`
- Node.js

```js
assert.notStrictEqual(value, true)
```

- Chai

```js
assert.isNotTrue(value)
```

### `value` is `false`
- Node.js

```js
assert.strictEqual(value, false)
```

- Chai

```js
assert.isFalse(value)
```

### `value` is not `false`
- Node.js

```js
assert.notStrictEqual(value, false)
```

- Chai

```js
assert.isNotFalse(value)
```

## number
### `value` is number
- Node.js

```js
assert.strictEqual(typeof value, 'number')
```

- Chai

```js
assert.isNumber(value)
```

### `value` is not number
- Node.js

```js
assert.notStrictEqual(typeof value, 'number')
```

- Chai

```js
assert.isNotNumber(value)
```

### `value` is `NaN`
- Node.js

```js
assert(Number.isNaN(value))
```

- Chai

```js
assert.isNaN(value)
```

- Jest

```js
expect(value).toBeNaN()
```

### `value` is not `NaN`
- Node.js

```js
assert(!Number.isNaN(value))
```

- Chai

```js
assert.isNotNaN(value)
```

### `value` is greater than `other`
- Node.js

```js
assert(value > other)
```

- Chai

```js
assert.isAbove(value, other)
```

- Jest

```js
expect(value).toBeGreaterThan(other)
```

### `value` is greater than or equal to `other`
- Node.js

```js
assert(value >= other)
```

- Chai

```js
assert.isAtLeast(value, other)
```

- Jest

```js
expect(value).toBeGreaterThanOrEqual(other)
```

### `value` is less than `other`
- Node.js

```js
assert(value < other)
```

- Chai

```js
assert.isBelow(value, other)
```

- Jest

```js
expect(value).toBeLessThan(other)
```

### `value` is less than or equal to `other`
- Node.js

```js
assert(value <= other)
```

- Chai

```js
assert.isAtMost(value, other)
```

- Jest

```js
expect(value).toBeLessThanOrEqual(other)
```

## string
### `value` is string
- Node.js

```js
assert.strictEqual(typeof value, 'string')
```

- Chai

```js
assert.isString(value)
```

### `value` is not string
- Node.js

```js
assert.notStrictEqual(typeof value, 'string')
```

- Chai

```js
assert.isNotString(value)
```

### `value` is empty
- Node.js

```js

assert.strictEqual(value.length, 0)
```

- Chai

```js
assert.isEmpty(value)
```

### `value` is not empty
- Node.js

```js

assert.notStrictEqual(value.length, 0)
```

- Chai

```js
assert.isNotEmpty(value)
```

### `value` has `length`
- Node.js

```js

assert.strictEqual(value.length, length)
```

- Chai

```js
assert.lengthOf(value, length)
```

- Jest

```js
expect(value).toHaveLength(length)
```

### `value` includes `other`
- Node.js

```js

assert(value.includes(other))
```

- Chai

```js
assert.include(value, other)
```

- Jest

```js
expect(value).toContain(other)
```

### `value` does not include `other`
- Node.js

```js

assert(!value.includes(other))
```

- Chai

```js
assert.notInclude(value, other)
```

### `value` matches to `pattern`
- Node.js

```js

assert(value.match(pattern))
```

- Chai

```js
assert.match(value, pattern)
```

- Jest

```js
expect(value).toMatch(pattern)
```

### `value` does not match to `pattern`
- Node.js

```js

assert(!value.match(pattern))
```

- Chai

```js
assert.notMatch(value, pattern)
```

## function
### `value` is function
- Node.js

```js
assert.strictEqual(typeof value, 'function')
```

- Chai

```js
assert.isFunction(value)
```

### `value` is not function
- Node.js

```js
assert.notStrictEqual(typeof value, 'function')
```

- Chai

```js
assert.isNotFunction(value)
```
## Array
### `value` is Array
- Node.js

```js
assert(Array.isArray(value))
```

- Chai

```js
assert.isArray(value)
```

### `value` is not Array
- Node.js

```js
assert(!Array.isArray(value))
```

- Chai

```js
assert.isNotArray(value)
```

### `value` is empty
- Node.js

```js

assert.strictEqual(value.length, 0)
```

- Chai

```js
assert.isEmpty(value)
```

### `value` is not empty
- Node.js

```js

assert.notStrictEqual(value.length, 0)
```

- Chai

```js
assert.isNotEmpty(value)
```

### `value` has `length`
- Node.js

```js

assert.strictEqual(value.length, length)
```

- Chai

```js
assert.lengthOf(value, length)
```

- Jest

```js
expect(value).toHaveLength(length)
```

### `value` includes `element`
- Node.js

```js

assert(value.includes(element))
```

- Chai

```js
assert.include(value, element)
```

- Jest

```js
expect(value).toContain(element)
```

### `value` does not include `element`
- Node.js

```js

assert(!value.includes(element))
```

- Chai

```js
assert.notInclude(value, element)
```

## Set
### `value` is empty
- Node.js

```js

assert.strictEqual(value.size, 0)
```

- Chai

```js
assert.isEmpty(value)
```

### `value` is not empty
- Node.js

```js

assert.notStrictEqual(value.size, 0)
```

- Chai

```js
assert.isNotEmpty(value)
```

### `value` has `size`
- Node.js

```js

assert.strictEqual(value.size, size)
```

- Chai

```js
assert.lengthOf(value, size)
```

## Map
### `value` is empty
- Node.js

```js

assert.strictEqual(value.size, 0)
```

- Chai

```js
assert.isEmpty(value)
```

### `value` is not empty
- Node.js

```js

assert.notStrictEqual(value.size, 0)
```

- Chai

```js
assert.isNotEmpty(value)
```

### `value` has `size`
- Node.js

```js

assert.strictEqual(value.size, size)
```

- Chai

```js
assert.lengthOf(value, size)
```
