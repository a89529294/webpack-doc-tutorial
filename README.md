# Webpack Starter - Output Management

## Steps

1. In root folder run `npm init -y`.
2. Run `npm i lodash`.
3. Run `npm i -D webpack webpack-cli html-webpack-plugin`.

### Notes

1. _html-webpack-plugin_ is used to automatically generate the build html file.
2. Add `clean: true` to output object in webpack.config.js so webpack deletes everything in build dir before `npm run build`.
