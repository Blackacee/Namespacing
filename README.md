# Namespacing
 
//Before: antipattern 3 global variables
 var setActivePage = function () {};
 var getPage = function() {};
 var redirectPage = function() {};
//After: just 1 global variable, no function collision and more meaningful function names
 var NavigationNs = NavigationNs || {};
 NavigationNs.active = function() {}
 NavigationNs.pagination = function() {}
 NavigationNs.redirection = function() {}
