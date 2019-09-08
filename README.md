1. Create starter repo

```sh
gatsby new hello-world https://github.com/gatsbyjs/gatsby-starter-hello-world
cd hello-world
```

2. Copy an official plugin and install it

```sh
mkdir plugins
cp -r <gatsby_repo>/packages/gatsby-plugin-google-analytics plugins

cd plugins/gatsby-plugin-google-analytics
npm install
```

3. Add plugin as a local plugin in `gatsby-config.js`

```javascript
module.exports = {
  plugins: ["gatsby-plugin-google-analytics"],
}
```

4. Run `gatsby develop`

## Resulting warning

```
Module Warning (from ./node_modules/eslint-loader/index.js):

/Users/dskang/Code/tmp/gatsby-eslint-strict/plugins/gatsby-plugin-google-analytics/gatsby-browser.js
  1:1  warning  'use strict' is unnecessary inside of modules  strict

✖ 1 problem (0 errors, 1 warning)
  0 errors and 1 warning potentially fixable with the `--fix` option.
```
