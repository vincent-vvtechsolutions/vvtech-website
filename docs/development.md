# Development Setup Guide

This document describes the technical setup and development workflow for the **vvtech-website** project.

## Stack Overview
- **Framework**: [Next.js 15+](https://nextjs.org/) (App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/) (Strict Mode)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **UI Components**: [shadcn/ui](https://ui.shadcn.com/)
- **Package Manager**: [pnpm](https://pnpm.io/)
- **Testing**:
  - **Unit**: [Vitest](https://vitest.dev/)
  - **E2E**: [Playwright](https://playwright.dev/)
- **Linting & Formatting**: [ESLint](https://eslint.org/) + [Prettier](https://prettier.io/)

## Getting Started

### Prerequisites
- **Node.js**: v20 or later (v24.12.0 recommended)
- **pnpm**: v10 or later

### Installation
```bash
pnpm install
```

### Development Server
```bash
pnpm dev
```
The application will be available at `http://localhost:3000`.

## Scripts
- `pnpm dev`: Runs the development server.
- `pnpm build`: Builds the application for production.
- `pnpm start`: Starts the production server.
- `pnpm lint`: Runs ESLint checks.
- `pnpm format`: Formats code using Prettier.
- `pnpm test`: Runs unit tests once.
- `pnpm test:watch`: Runs unit tests in watch mode.
- `pnpm test:e2e`: Runs end-to-end tests with Playwright.

## Project Structure
- `src/app/`: Next.js App Router (pages and layouts).
- `src/components/`: Reusable UI components.
- `src/components/ui/`: shadcn/ui base components.
- `src/hooks/`: Custom React hooks.
- `src/lib/`: Utility functions (including `utils.ts` for Tailwind merge).
- `src/test/`: Unit test setup and examples.
- `tests/e2e/`: Playwright E2E tests.
- `public/`: Static assets.

## Configuration Files
- `tsconfig.json`: TypeScript configuration (Strict mode enabled).
- `eslint.config.mjs`: ESLint flat config with Prettier integration.
- `.prettierrc`: Prettier rules and Tailwind plugin.
- `vitest.config.ts`: Vitest unit test configuration.
- `playwright.config.ts`: Playwright E2E test configuration.
- `components.json`: shadcn/ui configuration.
