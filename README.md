# React (v18+), Typescript, Yarn & Lerna Monorepo

Starting point for a Typescript, React (v18+, *tested up to v18.1.0*), Yarn & Lerna monorepo project with full setup for ESLint and Prettier.

## Stack

This project is initialized with [Create React App](https://github.com/facebook/create-react-app) consisting of:

- TypeScript
- React (v18+, *tested up to v18.1.0*)
- react-scripts (react-scripts v5+, *tested up to v5.0.1*, from createReactApp)
- react-testing-library (not Enzyme)
- Yarn Workspaces (multiple packages architecture)
- Lerna (tool for managing the monorepo packages)
- SASS/SCSS
- ESLint
- Prettier

### Content

The project now consists of 3 packages.

- **www**: create-react-app with TypeScript (react v18+, react-scripts v5)
- **shared**: react components with TypeScript (react v18+)
- **utils**: shared functions with TypeScript

## Get Started

### Make sure you run Node.js v10.15+

To install check ([Node.js installation](https://nodejs.org/en/) or [Node Version Manager installation](https://github.com/nvm-sh/nvm)).

### Clone or copy this repo

```bash
git clone git@github.com:darkspike13/react-ts-monorepo-boilerplate.git my_mono_repo
cd my_mono_repo
```


### `yarn install`

Note: this project is initialized with Yarn.

### Adding / removing packages

To add a new package create a new folder in under `packages` and copy the<br>
`.eslint.json`, `package.json`, `tsconfig.json` from another similar project in here.<br>
After that you can setup your project how you like it.

(you can also extend the custom scripts from the main `package.json`<br>
or already include in as dependency for another package).

After changing the packages run `yarn clean:update` to clean & reinit the workspaces.

After changing the external libraries or peerDependencies it is good to clean the repo<br>
by removing the node_modules folder `rm -rf node_modules` and reinstalling `yarn install`.
And after that run `yarn clean:update` to clean & reinit the workspaces.

## Development Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `yarn typecheck`

Launches the typescript check for code to check for TypeScript compilation errors or warnings.

### `yarn lint`

Launches the linter for code to check for code layout errors or warnings.

### `yarn lint:fix`

Launches the linter for code to check for code layout errors or warnings, and fixes the ones that can be fixed automatically.

### `yarn test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

## Production Scripts

### `yarn build`

Builds the app for production to the build folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
