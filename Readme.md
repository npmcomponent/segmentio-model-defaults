*This repository is a mirror of the [component](http://component.io) module [segmentio/model-defaults](http://github.com/segmentio/model-defaults). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/segmentio-model-defaults`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# model-defaults

  Lets a model specify default attribute values.

## Installation

    $ component install segmentio/model-defaults
    $ npm install model-defaults

## API

```js
var defaults = require('model-defaults')
  , model = require('model');

// all specified up front
var person = model('person')
  .use(defaults({
    name: '',
    age: 0
  }))
  .attr('name')
  .attr('age');

// or specified individually
var person = model
  .use(defaults)
  .attr('name', { default: '' })
  .attr('age', { default: 0 });
```

## License

  MIT
