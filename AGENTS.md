# Health In Hand Project - Agent Guidelines

## Commands
- `npm run dev` - Start dev server with Turbopack
- `npm run build` - Build production version  
- `npm run lint` - Run ESLint, `npm run lint:fix` - Auto-fix
- `npm run type-check` - TypeScript checking
- `npm run check` - Run lint + type-check (pre-commit required)
- `npm run check:fix` - Fix issues then check

## Code Style
**Imports:** Absolute imports with `@/` alias, grouped by type (React, third-party, local)
**Naming:** PascalCase components, camelCase functions/variables, UPPER_SNAKE_CASE constants
**Types:** Use `import type` for type-only imports, strict TypeScript with interfaces
**Components:** Server components by default, `"use client"` for interactivity, forwardRef for UI components
**Styling:** Use `cn()` utility for conditional Tailwind classes, shadcn/ui patterns
**Error Handling:** Try-catch with user-friendly messages, console.error for debugging
**Files:** Feature-based structure, clear separation between components, pages, lib, types

## Pre-commit Workflow
Always run `npm run check` before committing. Use `npm run check:fix` if issues exist.