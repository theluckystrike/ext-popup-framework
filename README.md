# ext-popup-framework

Chrome Extension Library by theluckystrike

## Overview

ext-popup-framework is a TypeScript library for building Chrome extension popups. It provides foundational types and utilities for extension development.

## Installation

```bash
npm install @theluckystrike/ext-popup-framework
```

## Usage

```typescript
import { extPopupFramework, VERSION } from '@theluckystrike/ext-popup-framework';

console.log(extPopupFramework); // "library"
console.log(VERSION); // "1.0.0"
```

## Development

```bash
# Clone the repository
git clone https://github.com/theluckystrike/ext-popup-framework.git
cd ext-popup-framework

# Install dependencies
npm install

# Build the project
npm run build

# Run tests
npm test
```

## API Reference

### Constants

| Export | Type | Description |
|--------|------|-------------|
| extPopupFramework | string | Library identifier |
| VERSION | string | Current version number |

## Related Packages

This package is part of the Zovo extension ecosystem:

- ext-popup-ui - UI components for popups
- ext-popup-page - Full popup page
- ext-popup-lib - Popup utilities

## Contributing

Contributions are welcome. Please see CONTRIBUTING.md for details.

## About

Built by theluckystrike. Part of the Zovo developer tools family at zovo.one.

## License

MIT - Copyright (c) 2025 theluckystrike
