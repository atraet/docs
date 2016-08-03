## Basic Builds with Webpack

To run Webpack, the following needed
- nodejs
- webpack (installed globally)


### CLI basics

```
webpack <source-file> <dest-file>
```

### Config file

When use config file, just run command *webpack*

```
module.exports = {
    entry: "./app.js",
    output: {
        filename: './dist/bundle.js'
    }
};
```

### Watch mode and the Webpack dev server
To enable watch mode, 2 ways
- --watch in command line
- watch: true in config file

file protocol vs http protocol
file:////
http://


Webpack dev server

- install

```
npm install webpack-dev-server -g
```

- run webpack dev server
```
webpack-dev-server --port <port-number>

-- inline (live reload)

```

go to
- http://localhost:8080/webpack-dev-server  (with status bar on top, live reload enabled)
- http://localhost:8080

### Building multiple files

### Using loaders

### Using pre-loaders

### Creating start scripts

### Production vs. Dev Builds
Production config
- Create a production config file, to extend/overwrite the dev config
- In production config, add a loader to strip all 'console.log',
- Push the strip-loader config to extend dev config

#### 3 npm servers
- http-server
- json-server
- webpack-dev-server

## Advanced Builds with Webpack

### Organizing Files and Folders

Webpack configuration properties
- context: directory of source files
- output.path
- output.publicPath: alias to the real file

### Working with ES6 modules
- extension .js --> .es6
- resolve.extensions: ['', 'js', 'es6']

### Advanced source maps
```
webpack -d -p
-d //debugger
-p //pretty display
```
### Multiple bundles

plugin **webpack.optimize.CommonsChunckPlugin('shared.js')**
