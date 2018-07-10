[![Build status](https://travis-ci.org/TherapyChat/copy-to-clipboard.svg?branch=master)](https://travis-ci.org/TherapyChat/copy-to-clipboard)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/therapychat/copy-to-clipboard)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com)

# \<copy-to-clipboard\>

Web Component to use [clipboard.js](https://clipboardjs.com/)

Example of use:
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="../paper-input/paper-input.html">
    <link rel="import" href="../paper-button/paper-button.html">
    <link rel="import" href="copy-to-clipboard.html">

    <next-code-block></next-code-block>

  </template>
</custom-element-demo>
```
-->
```html
<copy-to-clipboard
  id="copyToClipboard"
  clipboard-value-to-copy="[[value]]"
  clipboard-value-copied="{{copiedValue}}"
  clipboard-trigger-id="copyButton"
></copy-to-clipboard>
<paper-input
  label="Value to Copy"
  value="{{value}}"
></paper-input>
<paper-input
  label="Copied Value"
  value="[[copiedValue]]"
  disabled
></paper-input>
<paper-button id="copyButton">COPY</paper-button>
```

## Changelog

See [CHANGELOG](./CHANGELOG.md) file.

## Contributing

Please read [CONTRIBUTING](./CONTRIBUTING.md) file to follow good practices.

You will need [NodeJS](https://nodejs.org).

1. Close the repo: `git clone git@github.com:TherapyChat/copy-to-clipboard.git`
1. Install dependencies: `npm install`
1. Code!
1. Test: `npm test`
1. Create a [Pull Request](https://github.com/therapychat/copy-to-clipboard/pulls)

### Contributors

- [Alberto Fernandez](https://github.com/AlbertoFdzM)

## License

This project is available under the `Apache License 2.0`. See the [LICENSE](./LICENSE) file for more info.
