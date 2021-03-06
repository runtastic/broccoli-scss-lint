# broccoli-scss-lint 

> Broccoli plugin for validate .scss files

### Dependencies

1. [Ruby](http://www.ruby-lang.org/en/downloads/) (Ruby 1.9.3+)
2. [scss-lint](https://github.com/causes/scss-lint#installation)

### Installation
```shell
nmp install broccoli-scss-lint 
```

### Options

#### config
Type: `String`  
Default: `''`

Specify a configuration file to use

#### format
Type: `String`  
Default: `Default`

Output format (xml, config). If value of this option equals xml, option 'reportFile' cannot be empty

#### reportFile
Type: `String`  
Default: `''`

File where will be saved report

### Examples
1.
```js
var scssLint = require('broccoli-scss-lint');

// Validate with custom config
files = scssLint(tree, {
  config: '.config.yml'
});

```

2.
```js
var scssLint = require('broccoli-scss-lint');

// Save xml report
files = scssLint(tree, {
  format: 'xml',
  reportFile: 'scss-lint-report.xml'
});
```

### Release History

0.0.1 - First release