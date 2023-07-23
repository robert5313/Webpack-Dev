##### Loading CSS
## npm install --save-dev style-loader css-loader

# webpack.config.js
...code
module.exports = {
    mode: "development" or "production"
},
  module: {

    rules: [

      {

        test: /\.css$/i,

        use: ['style-loader', 'css-loader'],

      },

    ],

  },
 


The above order of loaders should be maintained: 'style-loader' comes first and followed by 'css-loader'. If this convention is not followed, webpack is likely to throw errors.


## Load Images
The image element will be display beside the text while the dist directory somethin like this 29822eaa871e8eadeaa4.png

the webpack found our file in src folder and processed it.


Every time we want to compile your code
##  npm run build

The different options available in webpack which helps to automatically compile our code

    webpack's Watch Mode
    webpack-dev-server
    webpack-dev-middleware

##  Using Watch Mode
We can instract webpack to watch all the files within our dependency graph for changes.

If one of the files is updated, the code will be recompiled we will not need to run the full build manually
add
 "watch": "webpack --watch",
 to Package.json file
We run # npm run watch

The webpack automatically recompiles the changed module!
but the downside is that we have to refresh our browser in order to see the changes.