# jsonata-moment
Moment.js support for [JSONata](http://jsonata.org/).

## How to install
```
npm install @elastic.io/jsonata-moment
```

## Usage
`$moment` function provides the same functionality, as regular `moment()` does.

#### In node.js

```javascript
const jsonataMoment = require('@elastic.io/jsonata-moment');
const result = jsonataMoment('$moment().format("YYYY-MM-DD")').evaluate();
```

#### In browser
There is a regular as well as minified versions of the library in a `dist` folder.

```javascript
const result = window.jsonataMoment('$moment().format("YYYY-MM-DD")').evaluate();
```