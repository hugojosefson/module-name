# module-name

Figures out the module name from the path of a script file.

Mostly the same as
[path.basename](https://nodejs.org/api/path.html#path_path_basename_p_ext), but
strips any extension. `module-name` also interprets
`deep/big/submodule/index.js` as `submodule` (rather than `index`).

## Installation

    npm install --save module-name

## Usage

    var moduleName = require('module-name');
    console.log('The name of this file module is ' + moduleName(__filename)); 
