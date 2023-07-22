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


