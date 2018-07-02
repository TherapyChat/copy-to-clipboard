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
    <dom-module id="app-element">
      <template>
        <next-code-block></next-code-block>
      </template>
      <script>
        Polymer({
          is: 'app-element',

          properties: {
            value: String,
            copiedValue: String
          },

          onClickCopy: function () {
            this.$.copyToClipboard.copy()
          }
        })
      </script>
    </dom-module>

    <app-element></app-element>
  </template>
</custom-element-demo>
```
-->
```html
<copy-to-clipboard
  id="copyToClipboard"
  value="{{value}}"
  clipboard-copied-value="{{copiedValue}}"
></copy-to-clipboard>
<paper-input value="[[value]]"></paper-input>
<paper-input value="{{copiedValue}}" read-only>
<paper-button on-click="onClickCopy">COPY</paper-button>
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
