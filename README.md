# node-date-stream
Provides an automated rotational stream based on date.

## Usage

```js
var dateStream = require('date-stream');
var stream = dateStream.getStream('access.log', 'yyyymmdd');
// express/morgan
app.use(morgan('combined', {stream: stream}));
```

## API

### .getStream(filename, format, timezone, separator)

#### filename

Type: `String`

#### format

Type: `String`

Default: `yyyymmdd`

#### timezone

Type: `Number`

Default: `8`

#### separator

Type: `String`

Default: `-`
