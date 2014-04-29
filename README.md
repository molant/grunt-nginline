# grunt-nginline

> Takes the content of templateUrl of a directive and puts it into the template property

## Getting Started
This plugin requires Grunt.

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install inline-angular-templates --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('inline-angular-templates');
```

## The "nginline" task

### Overview
In your project's Gruntfile, add a section named `inline_angular_templates` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  nginline: {
    dist: {
        templates: ['tmp/templates/'], //Where all the templates are
        src: ['tmp/directives/*.js'] // The path to the directives to process
    }
  },
})
```

This task will modify the src files. It is meant to be used in combination with other grunt tasks like ngmin or concat.

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_

## License
Copyright (c) 2014 molant. Licensed under the MIT license.
