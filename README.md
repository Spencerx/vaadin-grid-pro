# &lt;vaadin-grid-pro&gt;

> ⚠️ Starting from Vaadin 20, the source code and issues for this component are migrated to the [`vaadin/web-components`](https://github.com/vaadin/web-components/tree/master/packages/vaadin-grid-pro) monorepository.
> This repository contains the source code and releases of `<vaadin-grid-pro>` for the Vaadin versions 10 to 19.

[&lt;vaadin-grid-pro&gt;](https://vaadin.com/components/vaadin-grid-pro) is a high quality data grid / data table Web Component with extended functionality, part of the [Vaadin components](https://vaadin.com/components).

[Live Demo ↗](https://vaadin.com/components/vaadin-grid-pro/html-examples)
|
[API documentation ↗](https://vaadin.com/components/vaadin-grid-pro/html-api)

[![npm version](https://badgen.net/npm/v/@vaadin/vaadin-grid-pro)](https://www.npmjs.com/package/@vaadin/vaadin-grid-pro)
[![Published on Vaadin Directory](https://img.shields.io/badge/Vaadin%20Directory-published-00b4f0.svg)](https://vaadin.com/directory/component/vaadinvaadin-grid-pro)
[![Discord](https://img.shields.io/discord/732335336448852018?label=discord)](https://discord.gg/PHmkCKC)

<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="vaadin-grid-pro.html">
    <link rel="import" href="vaadin-grid-pro-edit-column.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<vaadin-grid-pro>
  <vaadin-grid-pro-edit-column path="firstName" header="First Name"></vaadin-grid-pro-edit-column>
  <vaadin-grid-pro-edit-column path="lastName" header="Last Name"></vaadin-grid-pro-edit-column>
  <vaadin-grid-pro-edit-column path="email" header="Email"></vaadin-grid-pro-edit-column>
</vaadin-grid-pro>
<script>
  // Populate the grid with data
  const grid = document.querySelector('vaadin-grid-pro');
  fetch('https://demo.vaadin.com/demo-data/1.0/people?count=200')
    .then(res => res.json())
    .then(json => grid.items = json.result);
</script>
```

[<img src="https://raw.githubusercontent.com/vaadin/vaadin-grid-pro/master/screenshot.png" width="900" alt="Screenshot of vaadin-grid-pro">](https://vaadin.com/components/vaadin-grid-pro)


## Installation

The Vaadin components are distributed as Bower and npm packages.
Please note that the version range is the same, as the API has not changed.
You should not mix Bower and npm versions in the same application, though.

Unlike the official Polymer Elements, the converted Polymer 3 compatible Vaadin components
are only published on npm, not pushed to GitHub repositories.

### Polymer 2 and HTML Imports compatible version

Install `vaadin-grid-pro`:

```sh
bower i vaadin/vaadin-grid-pro --save
```

Once installed, import it in your application:

```html
<link rel="import" href="bower_components/vaadin-grid-pro/vaadin-grid-pro.html">
```
### Polymer 3 and ES Modules compatible version


Install `vaadin-grid-pro`:

```sh
npm i @vaadin/vaadin-grid-pro --save
```

Once installed, import it in your application:

```js
import '@vaadin/vaadin-grid-pro/vaadin-grid-pro.js';
```

## Getting started

Vaadin components use the Lumo theme by default.

To use the Material theme, import the correspondent file from the `theme/material` folder.

## Entry points

- The component with the Lumo theme:

  `theme/lumo/vaadin-grid-pro.html`

- The component with the Material theme:

  `theme/material/vaadin-grid-pro.html`

- Alias for `theme/lumo/vaadin-grid-pro.html`:

  `vaadin-grid-pro.html`


## Running demos and tests in a browser

1. Fork the `vaadin-grid-pro` repository and clone it locally.

1. Make sure you have [npm](https://www.npmjs.com/) and [Bower](https://bower.io) installed.

1. When in the `vaadin-grid-pro` directory, run `npm install` and then `bower install` to install dependencies.

1. Make sure you have [polymer-cli](https://www.npmjs.com/package/polymer-cli) installed globally: `npm i -g polymer-cli`.

1. Run `npm start`, browser will automatically open the component API documentation.

1. You can also open demo or in-browser tests by adding **demo** or **test** to the URL, for example:

  - http://127.0.0.1:3000/components/vaadin-grid-pro/demo
  - http://127.0.0.1:3000/components/vaadin-grid-pro/test


## Running tests from the command line

> [!WARNING]
> Running tests locally from the CLI does not work due to outdated dependencies. Run tests via SauceLabs or in the browser instead.

1. When in the `vaadin-grid-pro` directory, run `polymer test`


## Following the coding style

We are using [ESLint](http://eslint.org/) for linting JavaScript code. You can check if your code is following our standards by running `npm run lint`, which will automatically lint all `.js` files as well as JavaScript snippets inside `.html` files.


## Big Thanks

Cross-browser Testing Platform and Open Source <3 Provided by [Sauce Labs](https://saucelabs.com).


## Contributing

  To contribute to the component, please read [the guideline](https://github.com/vaadin/vaadin-core/blob/master/CONTRIBUTING.md) first.


## License

Commercial Vaadin Add-on License version 3 (CVALv3). For license terms, see LICENSE.

Vaadin collects development time usage statistics to improve this product. For details and to opt-out, see https://github.com/vaadin/vaadin-usage-statistics.
