# Webpack Starter

## Steps

1. In root folder run `npm init -y`.
2. Run `npm i -D webpack webpack-cli css-loader style-loader csv-loader xml-loader`.
   - webpack-cli is for issuing webpack commands.
   - see webpack.config.js for how to configure the loaders.

### Notes

1. Loaders in webpack: Webpack only understands JS and JSON file out of the box. _Loaders_ allow webpack to process other types of files.
   - Add loaders into `module.exports.module` object in `webpack.config.js`.
   - It takes two properties, _test_ identifies which files to transform, _use_ indicates which loader to use.
2. You can also use `asset/resource` and friends to tell webpack how to handle assets w/o using loaders.
   - `asset/resource` emits a separate file and exports the URL. Same as the loader `file-loader`.
   - `asset/inline` exports a data uri of the asset. Same as the loader `url-loader`.
   - `asset/source` exports the source code of the asset. Same as the loader `raw-loader`.
   - `asset` automatically chooses between option 1 and 2.
