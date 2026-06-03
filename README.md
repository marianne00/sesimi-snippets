# Galaxy Snippets

VS Code snippet extension for Galaxy template development at Sesimi.

## Snippets

### TypeScript & TypeScript React (`.ts`, `.tsx`)

| Prefix | Description |
|--------|-------------|
| `glxUrlStatus` | Hook to check the loading status of a URL |

### TypeScript (`.ts`)

| Prefix | Description |
|--------|-------------|
| `glxContext` | Galaxy Page Context Hook with dev environment check |
| `glxActivePreset` | Function to determine the active preset based on aspect ratio |
| `glxHook` | Galaxy Template Hook Boilerplate |

### TypeScript React (`.tsx`)

| Prefix | Description |
|--------|-------------|
| `glxComponent` | React component with `cn` utility |

## Usage

Open a `.ts` or `.tsx` file, type a prefix, and press `Tab` or `Enter` to expand. Use `Tab` to navigate between placeholder fields.

**Example** — type `glxContext` and press `Tab`:

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

### From VSIX

1. Download the `.vsix` from [releases](https://github.com/marianne00/galaxy-snippets)
2. Open VS Code → Extensions (`Cmd+Shift+X` / `Ctrl+Shift+X`)
3. Click `...` → **Install from VSIX...**
4. Select the downloaded file

### From the command line

```bash
code --install-extension galaxy-snippets-1.0.0.vsix
```

## Requirements

VS Code 1.80.0 or higher.

---

Maintained for internal use at Sesimi. For suggestions, reach out to [Marianne](mailto:mdeasis@sesimi.com).
