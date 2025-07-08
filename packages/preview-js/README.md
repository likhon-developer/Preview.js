# @likhonsheikhofficial/preview-js

An advanced in-browser sandbox for AI agents and live coding. Run any Node.js app in any browser, powered by WebContainers.

## Installation

```bash
npm install @likhonsheikhofficial/preview-js
# or
yarn add @likhonsheikhofficial/preview-js
```

## Usage

This package provides a React component `PreviewProvider` and hooks to interact with a WebContainer-based sandbox.

### `PreviewProvider`

Wrap your application with `PreviewProvider` to enable the sandbox functionality.

```tsx
import { PreviewProvider } from '@likhonsheikhofficial/preview-js';
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';

ReactDOM.createRoot(document.getElementById('root')!).render(
  <React.StrictMode>
    <PreviewProvider>
      <App />
    </PreviewProvider>
  </React.StrictMode>,
);
```

### Hooks

- `useWebContainer()`: Provides access to the WebContainer instance.
- `useFileSystem()`: Provides utilities to interact with the in-browser file system.
- `useTerminal()`: Provides utilities to interact with the in-browser terminal.

## Development

To build the package:

```bash
npm run build
```

To run in development mode (watches for changes):

```bash
npm run dev
```

## Contributing

Contributions are welcome! Please see the main project's `README.md` for more details on how to contribute.

## License

MIT