# building

## required tooling

building the editor requires installing `node`, `yarn`, and `react-scripts`.

- `npm install -g yarn` (or brew install yarn)
- `npm install -g react-scripts`

## to build

```
yarn install
yarn build
```
running `yarn build` will output static, bundled, and minified js, css, and html files suitable for release in the `build` directory. the built results are self contained and do not depend on node or any of the associated react toolchain.

## development and testing

running `yarn start` starts a local development server which automatically recompiles (and reloads) the application when a file is saved.

the development server runs on port 3000 and forwards any unhandled request to the `"proxy"` defined in the `package.json` file. starting the `norns-web` server in a separate shell allows api calls to be handled during development.
