# Angular JS Debug Mode

1. Issue
2. Solution
3. Example
4. References
5. Keywords


## 1. Issue

AngularJS by default adds scope references to the DOM for tools such as angularjs-batarang to work. This has an impact on your application performance.

## 2. Solution

It can be `disabled` using the `$compileProvider` provider:

## 3. Example

```javascript
angular.module('yourModule').config(function($compileProvider) {
    if (/* test if in production */) {
        $compileProvider.debugInfoEnabled(false);
    }
});
```

## 4. References

[1] http://julienrenaux.fr/2015/08/24/ultimate-angularjs-and-ionic-performance-cheat-sheet/#Debug

## 5. Keywords
`angularjs` `angularjs performance` `angularjs debug`
