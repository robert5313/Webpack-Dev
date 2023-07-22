# WHEN we use print.js

## when we click the button we get print.js being counted by the number of clicks we make
## Setting up HtmlWebpackPlugin
## npm install --save-dev html-webpack-plugin

  plugins: [

    new HtmlWebpackPlugin({

      title: 'Output Management',

    }),

  ],

  HtmlWebpackPlugin by default will generate its own index.html
  In dist/ folder
  It is good practice to clean the /dist folder before each build.


     output: {
++   clean: true,
   },

## npm run build
It will create index.html in dist folder but if it is already available it will overwrite 