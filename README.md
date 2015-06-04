# grunt-velocity

> Grunt plugin to run the velocity templates through the node velocity engine in an un-opinionated way.

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-velocity --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-velocity');
```

## The "velocity" task

### Overview
In your project's Gruntfile, add a section named `velocity` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  velocity: {
    options: {
      data: path/to/data.json
    },
    files: {
      <standard grunt dest & source file specification>
    }
});
```

### Options

#### options.data
Type: `String`

A path to the data (JSON) file that will be merged with the templates.


### Usage Examples

#### Options
In this example, the data (JSON file or JSON Object) is specified in the options, and the velocity templates (that consume the data) & output folder are specified in the task.
The example below is in the grunt format, of dest: [src files], but any standard grunt format can be used.

```js
grunt.initConfig({
  velocity: {
     options: {
        data: 'path/to/data.json' // alternately {}
     },
     files: {
      'my/output_folder/': ['src/velocity-templates/**/*.vm']
     }
  }
});
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_
