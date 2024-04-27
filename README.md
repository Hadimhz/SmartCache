# SmartCache

SmartCache is a simple, efficient caching system implemented in TypeScript.

## Features

- Customizable cache expiry times
- Option to keep expired cache data
- Callback function for when data is removed
- Regular cache invalidation

## Installation

Use the package manager [npm](https://www.npmjs.com/) to install SmartCache.

```bash
npm install smartcache
```

## Usage

```javascript
import Cache from 'smartcache';

const cache = new Cache();

// Set a value in the cache
cache.set('key', 'value', 10000); // Expires in 10 seconds

// Get a value from the cache
let value = cache.get('key'); // Returns 'value' or undefined if not found or expired

// Get the raw cache value
let rawValue = cache.get('key', { raw: true }); // Returns the CacheValue object or undefined
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://opensource.org/licenses/MIT)