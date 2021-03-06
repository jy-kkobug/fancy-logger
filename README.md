# Fancy Logger

Fancy Logger is logging library for browser.

## Installation

```bash
// npm
npm i @jy-kkobug/fancy-logger

// yarn
yarn add @jy-kkobug/fancy-logger

// pnpm
pnpm i @jy-kkobug/fancy-logger
```

## Usage

```typescript
import FancyLogger, { LoggerColor } from '@jy-kkobug/fancy-logger';

const logger = FancyLogger.getInstance();

logger.debug('test');
logger.trace('test');
logger.error('test');
logger.warn('test');
logger.log('test', 'group:tag1', LoggerColor.Purple);
logger.log('test', 'group:tag2', LoggerColor.NeonBlue);

console.log(logger.getLogs());

logger.startRecord();

logger.debug('test');
logger.trace('test');
logger.error('test');
logger.warn('test');
logger.log('test', 'group:tag1', LoggerColor.Purple);
logger.log('test', 'group:tag2', LoggerColor.NeonBlue);

logger.stopRecord();

console.log(logger.getLogs());
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
