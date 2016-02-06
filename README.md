# angular-d3-module
Angular D3 module to load D3 library in Angular controllers.

Inspired by [Angular-underscore-module](https://github.com/andresesfm/angular-underscore-module])

## Setup

### 1. Include D3 first in your project
``` <script src="bower_components/d3/d3.js"> ```

### 2. Install Angular-d3
``` bower install angular-d3-module ```

### 3. Add Angular-d3 in your project
```<script src="bower_components/angular-d3-module/angular-d3-module.js"></script>```

## Use in Angular

### 1. Add the module in the dependancy

``` angular.module('myApp', ['d3'])```

### 2. Add as an injected dependency to Controller

``` 
angular.module('myApp')
	.controller('ChartCtrl', [
		'$scope', 
		'd3', 
		function ($scope, d3) {
			//code using d3 comes here
		}
	]);
```