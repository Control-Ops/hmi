# HMI

The Control Ops Human Machine Interface (HMI) provides a visual interface that allows users to:
1. Modify the control settings of plant unit operations
2. View the state of unit operations in real time
3. View historical data for unit operations

The HMI is a browser-based project built with the [Vue.js](https://vuejs.org/) framework and uses [Vite](https://vite.dev/) as the build tool.

## Recommended IDE Setup
- Paid: [WebStorm](https://www.jetbrains.com/webstorm/buy/?section=personal&billing=monthly) / [IntelliJ IDEA Ultimate](https://www.jetbrains.com/idea/buy/?section=personal&billing=yearly)
- Free, but buggy: [VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur)

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, `tsc` was replaced with `vue-tsc` in the CLI for type checking.

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup
The Node Package Manager (npm) is required to install the project's dependencies; [Node.js](https://nodejs.org/en) must be installed on your machine for the setup instructions to work. 

To set up the project, simply run the following command in the project's root directory:
```sh
npm install
```
This will install all project dependencies in one shot. 
## Useful Commands
Run the following commands in the project's root directory to do useful things:

### Compile and Launch a Hot-Reloaded Development Server

```sh
npm run dev
```
The development server will automatically recompile and refresh when source files are modified.

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
npm run test:unit
```

### Run End-to-End Tests with [Playwright](https://playwright.dev)

```sh
# Install browsers for the first run
npx playwright install

# When testing on CI, must build the project first
npm run build

# Runs the end-to-end tests
npm run test:e2e
# Runs the tests only on Chromium
npm run test:e2e -- --project=chromium
# Runs the tests of a specific file
npm run test:e2e -- tests/example.spec.ts
# Runs the tests in debug mode
npm run test:e2e -- --debug
```
### Format Code with [Prettier](https://prettier.io/)

```sh
npm run format
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
