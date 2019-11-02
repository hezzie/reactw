# React App from scratch
# How to set up React.js app from scratch without using create-react-app?
Prerequisite
Node.js must be installed on your computer. I hope you guys are familiar with yarn. Also, yarn is installed globally.
Create an empty project and create a package.json file.
Installation
Install the following packages.

# Setup React.js
`yarn add react and react-dom`

react-dom - This package serves as the entry point to the DOM and server renderers for React.

# Setup webpack
`yarn add -D webpack -g webpack-cli -g webpack-dev-server -g html-webpack-plugin -g`
webpack - Webpack is a bundler for modules.

webpack-cli - Command Line interface for webpack.

webpack-dev-server - Development server that provides live reloading.

html-webpack-plugin - The HtmlWebpackPlugin simplifies creation of HTML files to serve your webpack bundles.

# Setup Babel
`yarn add -D @babel/core @babel/preset-env @babel/preset-react babel-loader`
@babel/core - Mainly used to convert ECMAScript 2015+ code into a backwards compatible version of JavaScript.

@babel/preset-env - @babel/preset-env allows you to use the latest JavaScript.

@babel/preset-react - This package is a set of plugins used to support React.js specific features.

babel-loader - This package allows transpiling JavaScript files using Babel and webpack.

# Configuration
We have installed all the required packages to create a React.js application using webpack.
Next we need an index.html template where we need to insert the react constructed dom. 
Create an HTML file inside src/ folder.

#src/index.html
  
Also, we need a starting point to create react application. Create a js file index src/ folder.

# src/index.js
  
# Configure webpack to serve live development server

# webpack.config.js

Babel Configurations

.babelrc
We have reached to the finishing line. Oh wait! there is one more thing to be done. Add the webpack scripts to package.json file.

# package.json
That's all! It's show time. Let's start the development server.


  `yarn serve`

