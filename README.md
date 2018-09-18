# angular-routing

server will ignore anything after a # in a route  
- (client side can the grab onto it)  
- [simplified idea]

You can have multiple controllers with different names in different divs. 

---
NEED:  
- `npm install angular`  
- `npm install angular-route`

> Make sure to then copy and paste from node_modules & source in. 

> And source in after angular but before client
---
- ngRoute as a new dependency in angular module

- give controller of a very specific part 
`ng-view`

can only have 1 config: 
```
colorApp.config(['$routeProvider', function($routeProvider) {
}])
```
but can have many controllers

---

Started with controllers on html for formating sack:
```
  <!-- Red Controller -->
  <div ng-controller="RedController as vm">
    <h1>{{vm.message}}</h1>
  </div>

  <!-- Blue Controller -->
  <div ng-controller="BlueController as vm">
    <h1>{{vm.message}}</h1>
  </div>
```
> then copy & paste with back ticks

---

then just move code around!

---
> change to templateUrl, give it the path in a string
---

each view will have its own controller
1-1