# unique-object-by

Filters an Object or Map by testing entry uniqueness with a callback.

This module is an alias of [`unique-map-by`](https://github.com/lamansky/unique-map-by), which supports both Maps and Objects.

## Installation

```bash
npm install unique-object-by --save
```

## Usage Example

```javascript
const uniqueObjectBy = require('unique-object-by')

const obj = {
  1: {name: 'John'},
  2: {name: 'John'},
  3: {name: 'Stephen'},
}

const u = uniqueObjectBy(obj, (key, value) => value.name)
u[1] // {name: 'John'}
u[2] // undefined
u[3] // {name: 'Stephen'}
```

For more details, see the documentation for the [`unique-map-by`](https://github.com/lamansky/unique-map-by) module.
