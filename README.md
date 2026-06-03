# Galaxy Snippets

Company snippets for Sesimi development in VS Code.

## Features

This extension provides a collection of custom code snippets for TypeScript and TypeScript React development, specifically designed for Sesimi's Galaxy framework and component architecture.

## Available Snippets

### TypeScript Snippets

| Prefix | Description |
|--------|-------------|
| `glxContext` | Galaxy Page Context Hook with dev environment check |
| `glxActivePreset` | Function to determine the active preset based on aspect ratio |
| `glxHook` | Galaxy Template Hook Boilerplate |

### TypeScript & TypeScript React Snippets

| Prefix | Description |
|--------|-------------|
| `glxUrlStatus` | Hook to check the loading status of a URL |

### TypeScript React Snippets

| Prefix | Description |
|--------|-------------|
| `glxComponent` | Create a minimal React component with cn utility |

## Usage

1. Open a TypeScript or TypeScript React file (`.ts`, `.tsx`)
2. Start typing one of the snippet prefixes (e.g., `glxContext`)
3. Press `Tab` or `Enter` to expand the snippet
4. Use `Tab` to navigate between placeholder fields

### Example

Type `glxContext` and press `Tab` to generate:

```typescript
import { useContext } from 'react'
import { PageContext } from '../pages/001/data/context'

export function index() {
  const {  } = useContext(PageContext)
  const isDev = typeof import.meta !== 'undefined' && import.meta.env && import.meta.env.DEV === true

  if (isDev) {
    // Development environment specific code here
  }

  // return LIVE values here
}
```

## Installation

### From VSIX File

1. Download the `.vsix` file from the releases
2. Open VS Code
3. Go to Extensions view (`Cmd+Shift+X` on macOS, `Ctrl+Shift+X` on Windows/Linux)
4. Click the `...` menu at the top of the Extensions view
5. Select "Install from VSIX..."
6. Choose the downloaded `.vsix` file

### From Command Line

```bash
code --install-extension galaxy-snippets-1.0.0.vsix
```

## Requirements

- VS Code version 1.80.0 or higher

## Contributing

This extension is maintained for internal use at Sesimi. For suggestions or improvements, please contact the development team.

## Author

**Marianne**
Email: mdeasis@sesimi.com

## Repository

[GitHub Repository](https://github.com/marianne00/galaxy-snippets)

## Version History

### 1.0.0
- Initial release
- Added Galaxy framework snippets for TypeScript and TypeScript React
- Includes context hooks, components, and utility functions

---

**Enjoy coding with Galaxy Snippets!** 🚀
