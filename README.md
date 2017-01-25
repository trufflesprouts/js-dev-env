# js-dev-env
Starter ES6 development environment that handles bundling, linting, transpiling, testing, and much more.<br>


Requirements:<br>
1. Install Node 4 or greater (5 or greater recommended for optimum performance).<br>
2. Run ‘npm install’ in the root folder of each project.<br>

<sub><i>Keywords: ES6, Webpack, Babel, ESLint, Mocha, Chai, JSDOM, ngrok </i></sub>
<br>
### `npm start`
Runs the app in development mode.<br>
Specifically it runs security-check, ESLint, Mocha tests, MockApi and starts express development server on port 3000.<br>
Configure server in <i>buildScripts/srcServer.js</i>.

### `npm run share`
Starts dev server on port 3000 and exposes it using ngrok.<br>
You can also expose already running server on port 3000 with `npm run ngrok`.

### `npm run build`
Builds the app for production to the `dist` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.<br>
It also serves the build on port 3000, Configure server in <i>buildScripts/distServer.js</i>.

### `npm run deploy`
Uses surge to deploy static apps.
