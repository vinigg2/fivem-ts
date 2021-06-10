<h1 align="center">fivem-ts</h1>

<p align="center">
  <i>:video_game: A Typescript Template for FiveM :video_game:</i>
  <br>
  <br>
  <a href="https://github.com/vinigg2/fivem-ts/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat" alt="License: MIT">
  </a>
  <a href="https://github.com/vinigg2/fivem-ts/commits/master">
    <img src="https://img.shields.io/github/last-commit/vinigg2/fivem-ts.svg?style=flat" alt="Last commit">
  </a>
  <a href="">
    <img src="https://img.shields.io/github/workflow/status/vinigg2/fivem-ts/Node.js%20CI" alt="Workflow">
  </a>
</p>

This is a basic template for creating a FiveM resource using Typescript. It includes webpack config files, linting (ESlint + prettier) and a directory structure to get you started.

## Usage
1. Clone repository into your `resources/[local]` folder.
2. `npm i` the dependencies.
3. Start development.

### Development
Use `npm run watch` to watch files during development.

### Production
Build your production ready code with `npm run build`.

This will build the client and server script with the `--mode production` flag.

### Automatic Builds (Optional)
The `fxmanifest.lua` is not setup to automatically build upon first FXServer start. If you'd like to setup automatic builds you must add the following to your `fxmanifest.lua`.

```lua
dependency 'yarn'
dependency 'webpack'

webpack_config 'webpack.config.js'
```

However, due to the speed performance of the pre-packaged webpack/yarn of cfx-server-data, we suggest you don't do this and build manually as described previously ("Production").

## License
This product is MIT licensed. Please make sure you give credit and include this license in your product.