node-elasticsearch
============

This is a module around the REST API for [Elastic Search](http://www.elasticsearch.org/) built for NodeJS.


Details
=============

This works with node 0.4.x and with 0.2.x. I needed it for both and so wrote an [http compatability layer](http://github.com/ncb000gt/node-http_compat).


Usage
=============

     var lib = require('elasticsearch'), sys = require('sys'); //replace sys with util if you're on node 0.4.x
     lib.createClient(function(client) {
         client.query({query: {field: {field1: 'hai'}}}, function(err, results) {
             console.log(sys.inspect(results, true, 10));
         });
     });


API
==============

*Will go here when I'm ready to post it.*


Requirements
=============

* NodeJS
* Elastic Search
* nodeunit (for testing)
* The need for search


License
=============

MIT


Trademarks?
============

Node.js™ is an official trademark of Joyent. This module is not formally related to or endorsed by the official Joyent Node.js open source or commercial project