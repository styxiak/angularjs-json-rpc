AngularJS json rpc
==================
This code is far from the repository from which it was forked.
JSON-RPC-2.0 implementation for [AngularJS](http://angularjs.org/).

For Usage see `test.js`.

An example JSFiddle is working here: http://jsfiddle.net/89D4b/1/


Instead of creating a new factory for handling jsonrpc request, this angular module (angular-json-rpc) creates a new shortcut just like $http.get, but is instead $http.jsonrpc;


This code is under [WTFPL](http://www.wtfpl.net/).


Author
========
* By [cfairweather](https://www.github.com/cfairweather)

Example usage:
====

In your module, import 'angular-json-rpc':
        
        angular.module('test-module-jsonrpc', ['angular-json-rpc'])

Then:

        //url, method, parameters, config
        $http.jsonrpc('url/to/jsonrpc/service', 'methodToCall', [1, 2, 3], {}).success(function(){}).error(function(){});
For more information on callacks, see [$http](http://docs.angularjs.org/api/ng.$http).
