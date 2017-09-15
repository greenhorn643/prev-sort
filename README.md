# Prev Sort

## Installation

```shell
npm install --save prev-sort
```

## Usage

```javascript
import prevSort from 'prev-sort'

const array = [
  { id: 4, previousId: 3 },
  { id: 2, previousId: 1 },
  { id: 3, previousId: 2 },
  { id: 1, previousId: null },
]

const sortedArray = prevSort(array, {
  getId: (item) => item.id,
  getPreviousId: (item) => item.previousId,
})
```