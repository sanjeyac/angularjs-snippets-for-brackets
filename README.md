
# AngularJS code templates for Brackets

This is a set of snippets for [Brackets by Adobe](http://brackets.io/)

It contains the following skeletons, based on [John Papa's AngularJS Style Guide](https://github.com/johnpapa/angular-styleguide)

* controller
* directive
* factory
* filter
* module
* service

## Install

1. In order to install the snippets you have to install 'Brackets Snippets (by edc)' from the Extension manager ( File > Extension manager ) and download the [angularjsSnippets.yml from the repository](https://github.com/sanjeyac/angularjs-snippets-for-brackets)
2. After you have installed the Snippet Manager click on the Snippet Manager icon on the right side (a bulb)
3. A panel will appear on the bottom. Click on Settings and then on Import.
4. Select angularjsSnippets.yml from where you downloaded and it's done.

## Usage

Write 'ngcontroller' on a Javascript file to generate an AngularJS Controller skeleton,
press TAB to customize all the paramaters of the code.

The following elements works in the same way:
* ngcontroller - a controller
* ngdirective - a directive
* ngfactory - a factory
* ngfilter - a filter
* ngservice - a service
* ngapp - an angula module

## Generated snippets samples

```javascript
/* =================== CONTROLLER =================== */
(function() {
    'use strict';

    angular
        .module('module')
        .controller('Controller', Controller);

    Controller.$inject = ['dependencies'];

    /* @ngInject */
    function Controller(dependencies){
        var vm = this;
        vm.title = 'Controller';

        activate();

        ////////////////

        function activate() {
        }
    }
})();

/* =================== DIRECTIVE =================== */
(function () {
    'use strict';
    
    
    angular
        .module('module')
        .directive('directive', directive);
    
    directive.$inject = ['dependencies'];
    
    /* @ngInject */
    function  directive(dependencies) {
        // Usage:
        //
        // Creates:
        //
        var directive = {
            bindToController: true,
            controller: Controller,
            controllerAs: 'vm',
            link: link,
            restrict: 'A',
            scope: {}
        };
        return directive;

        function link(scope, element, attrs) {}
    }
    
    /* @ngInject */
    function Controller() {
    
    }

})();

/* =================== FACTORY =================== */
(function () {
    'use strict';
    angular
        .module('module')
        .factory('factory', factory);
    
    factory.$inject = ['dependencies'];
    
    /* @ngInject */
    function  Factory(dependencies){
        var service = {
            func: func
        };
    
        return service;
    
        ////////////////
        function func() {
            
        }
    }
})();

/* =================== APP MODULE =================== */
(function () {
    'use strict';

    angular
        .module('module', [
                                'dependencies'
                                ]);
})();

/* =================== FILTER =================== */
(function () {
    'use strict';
    angular
        .module('module')
        .filter('filter', filter);
    
    
    function filter() {
        return filterFilter;
        ////////////////
        
        function filterFilter(params) {
            return params;
        };
    }
})();

```

