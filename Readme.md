*This repository is a mirror of the [component](http://component.io) module [cristiandouce/loading-lock](http://github.com/cristiandouce/loading-lock). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/cristiandouce-loading-lock`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# loading-lock

  Loading lock component. Locks element while loading and adds spinner with [component/spin](https://github.com/component/spin).

  ![](http://d.pr/i/hFQ8+)


## Installation

    $ component install cristiandouce/loading-lock

## API
```js
  var loading = require('loading-lock');
```

### loading(el, options)
  Returns a `LoadingLock` instance for given element with options.
  Valid options are:
  * `size`: Size (Number) `diameter` of loading spinner.

```js
  var locker = loading(document.getElementById('example'), { size: 80 });
```

### .lock()
  Locks element adding 'locked' class and spinner.

```js
  locker.lock();
```

### .unlock()
  Unlocks element removing 'locked' class and spinner.

```js
  locker.unlock();
```

## License

  MIT
