# ext-popup-framework

[![npm version](https://img.shields.io/npm/v/@theluckystrike/ext-popup-framework)](https://npmjs.com/package/@theluckystrike/ext-popup-framework)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue.svg)](https://www.typescriptlang.org/)
[![CI Status](https://github.com/theluckystrike/ext-popup-framework/actions/workflows/ci.yml/badge.svg)](https://github.com/theluckystrike/ext-popup-framework/actions)
[![Discord](https://img.shields.io/badge/Discord-Zovo-blueviolet.svg?logo=discord)](https://discord.gg/zovo)
[![Website](https://img.shields.io/badge/Website-zovo.one-blue)](https://zovo.one)
[![GitHub Stars](https://img.shields.io/github/stars/theluckystrike/ext-popup-framework?style=social)](https://github.com/theluckystrike/ext-popup-framework)

> Framework for building modern Chrome extension popups.

Part of the [Zovo](https://zovo.one) family of privacy-first Chrome extensions and developer tools.

## Overview

`ext-popup-framework` is a comprehensive framework for building modern, responsive popup interfaces for Chrome extensions. It provides pre-built components, state management, and best practices for popup development.

## Features

- ✅ **Component-based** - React-like component architecture
- ✅ **TypeScript Support** - Fully typed for better developer experience
- ✅ **MV3 Compatible** - Works with Manifest V3 extensions
- ✅ **Responsive Design** - Mobile-friendly popup layouts
- ✅ **State Management** - Built-in state management
- ✅ **Privacy-First** - No data collection, all local

## Installation

### From npm

```bash
npm install @theluckystrike/ext-popup-framework
```

### From Source

```bash
# Clone the repository
git clone https://github.com/theluckystrike/ext-popup-framework.git
cd ext-popup-framework

# Install dependencies
npm install

# Build the project
npm run build
```

## Usage

### Basic Usage

```typescript
import { PopupApp, Button, Input } from '@theluckystrike/ext-popup-framework';

// Create a popup app
const app = new PopupApp({
  container: document.getElementById('popup')
});

// Add components
app.render([
  new Button({
    text: 'Click Me',
    onClick: () => console.log('Clicked!')
  }),
  new Input({
    placeholder: 'Enter text...'
  })
]);
```

### With State Management

```typescript
import { PopupApp, useState } from '@theluckystrike/ext-popup-framework';

const app = new PopupApp({
  container: document.getElementById('popup')
});

const [count, setCount] = useState(0);

app.render([
  new Button({
    text: `Count: ${count}`,
    onClick: () => setCount(count + 1)
  })
]);
```

## API Reference

### Components

| Component | Description |
|-----------|-------------|
| `PopupApp` | Main popup application container |
| `Button` | Interactive button component |
| `Input` | Text input component |
| `Card` | Card container component |
| `List` | List component |

### Hooks

| Hook | Description |
|------|-------------|
| `useState` | State management hook |
| `useEffect` | Side effects hook |
| `useStorage` | Chrome storage integration |

## Related Packages

This package is part of the Zovo extension UI ecosystem:

- [ext-popup-ui](https://github.com/theluckystrike/ext-popup-ui) - UI components for popups
- [ext-popup-page](https://github.com/theluckystrike/ext-popup-page) - Full popup page
- [ext-popup-lib](https://github.com/theluckystrike/ext-popup-lib) - Popup utilities
- [ext-options-page-ui](https://github.com/theluckystrike/ext-options-page-ui) - Options page UI

## Contributing

Contributions are welcome! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/popup-improvement`
3. **Make** your changes
4. **Test** your changes: `npm test`
5. **Commit** your changes: `git commit -m 'Add new feature'`
6. **Push** to the branch: `git push origin feature/popup-improvement`
7. **Submit** a Pull Request

### Development Setup

```bash
# Clone the repository
git clone https://github.com/theluckystrike/ext-popup-framework.git
cd ext-popup-framework

# Install dependencies
npm install

# Run tests
npm test

# Build
npm run build
```

## Built by Zovo

Part of the [Zovo](https://zovo.one) developer tools family — privacy-first Chrome extensions built by developers, for developers.

## See Also

### Related Zovo Repositories

- [zovo-extension-template](https://github.com/theluckystrike/zovo-extension-template) - Boilerplate for building privacy-first Chrome extensions
- [zovo-types-webext](https://github.com/theluckystrike/zovo-types-webext) - Comprehensive TypeScript type definitions for browser extensions
- [zovo-permissions-scanner](https://github.com/theluckystrike/zovo-permissions-scanner) - Privacy scanner for Chrome extensions
- [zovo-indexer](https://github.com/theluckystrike/zovo-indexer) - Indexing service for Zovo extensions

### Zovo Chrome Extensions

- [Zovo Tab Manager](https://chrome.google.com/webstore/detail/zovo-tab-manager) - Manage tabs efficiently
- [Zovo Focus](https://chrome.google.com/webstore/detail/zovo-focus) - Block distractions
- [Zovo Permissions Scanner](https://chrome.google.com/webstore/detail/zovo-permissions-scanner) - Check extension privacy grades

Visit [zovo.one](https://zovo.one) for more information.

## License

MIT - [Zovo](https://zovo.one)

---

*Built by developers, for developers. No compromises on privacy.*
