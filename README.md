# process-monitor

Monitors the CPU and memory usage for a PID or collection of PIDs.

## Getting Started
_(note: this module is not currently available in the npm registry)_

Install the module:

    npm install git://github.com/onmodulus/process-monitor.git#develop

Use it in your script:

    var procmon = require('process-monitor');
    procmon.monitor({ pid: process.id }).start();

## Documentation
Generated code documentation is available in the docs directory. This documentation is generated using
`docco-husky` - to regenerate the documentation, run `$ docco-husky lib/*`.

## Examples

    var procmon = require('./process-monitor').monitor({ pid: process.pid }).start();

    procmon.on('stats', function(stats) {
      console.dir(stats);
    });

## Release History
* 2012/09/14 - v0.1.0 - Initial release.

## License
Copyright (c) 2012 Modulus
Licensed under the MIT license.
