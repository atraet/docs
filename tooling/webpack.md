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
