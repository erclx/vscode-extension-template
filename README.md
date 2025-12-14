# VS Code Extension Template

A modern TypeScript template for building VS Code extensions with best practices baked in.

## What's Included

- **TypeScript** with strict type checking
- **esbuild** for fast bundling
- **ESLint + Prettier** for code quality and formatting
- **CSpell** for catching typos
- **Commitlint** for enforcing conventional commits
- **Auto-formatting** on save
- **Pre-configured workspace** settings and debug launcher

## Getting Started

1. **Clone the template**

   ```bash
   git clone <repository-url> my-extension
   cd my-extension
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Run the reset script**

   ```bash
   npm run reset
   ```

   This will prompt you for:
   - Extension display name
   - Extension identifier
   - Extension description

   Then it will update all metadata and reset the git history.

4. **Start developing**

   ```bash
   code .
   ```

   Press `F5` to launch the Extension Development Host and start debugging.

## Development

- **Compile**: `npm run compile` - Type check, lint, and bundle
- **Watch**: `npm run watch` - Auto-rebuild on file changes
- **Lint**: `npm run lint` - Check code quality
- **Spell check**: `npm run lint:spelling` - Catch typos
- **Test**: `npm test` - Run integration tests
- **Package**: `npm run package` - Build production bundle

All code is automatically formatted on save. Imports are auto-sorted by ESLint.

## Project Structure

```
.
├── .vscode/          # Workspace settings & debug config
├── src/
│   ├── extension.ts  # Main entry point
│   └── test/         # Integration tests
├── scripts/
│   └── reset.sh      # Template initialization script
└── package.json      # Extension manifest
```
