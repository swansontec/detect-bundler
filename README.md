# detect-bundler

This library exports two simple flags:

* `isBrowser` - True if a tool like [Webpack](https://webpack.js.org/) or [Browserify](http://browserify.org/) is bundling this project for the web.
* `isReactNative`- True if the [React Native](https://facebook.github.io/metro/) is bundling this project.

This library uses the [package.json browser field](https://github.com/defunctzombie/package-browser-field-spec) to select which flags to export. This means that everything happens at build time; there is no run-time platform detection.