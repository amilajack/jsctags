```js
var mod = window.mymodule

mod.func = function() { return 10 }

mod.func //: fn() -> number

var otherMod = window.yourmodule.theirmodule

otherMod.c = 10

otherMod.c //: number
```
```json
[
  {
    "id": "138207c0-7aef-11e6-95b5-9d06a43968d4",
    "name": "mod",
    "addr": "/mod/",
    "kind": "v",
    "lineno": 1,
    "origin": {
      "!span": "4[0:4]-7[0:7]",
      "!data": {
        "isConstructor": false
      }
    },
    "tagfile": "__DIR__/phantom_object.js"
  },
  {
    "id": "138255e0-7aef-11e6-95b5-9d06a43968d4",
    "name": "func",
    "addr": "/func/",
    "kind": "f",
    "type": "number function()",
    "lineno": 3,
    "namespace": "mod",
    "parent": "138207c0-7aef-11e6-95b5-9d06a43968d4",
    "origin": {
      "!span": "31[2:4]-35[2:8]",
      "!type": "fn() -> number",
      "!data": {
        "isConstructor": false,
        "type": "Function.prototype"
      }
    },
    "tagfile": "__DIR__/phantom_object.js"
  },
  {
    "id": "13827cf0-7aef-11e6-95b5-9d06a43968d4",
    "name": "otherMod",
    "addr": "/otherMod/",
    "kind": "v",
    "lineno": 7,
    "origin": {
      "!span": "97[6:4]-105[6:12]",
      "!data": {
        "isConstructor": false
      }
    },
    "tagfile": "__DIR__/phantom_object.js"
  },
  {
    "id": "13827cf1-7aef-11e6-95b5-9d06a43968d4",
    "name": "c",
    "addr": "/c/",
    "kind": "v",
    "type": "number",
    "lineno": 9,
    "namespace": "otherMod",
    "parent": "13827cf0-7aef-11e6-95b5-9d06a43968d4",
    "origin": {
      "!span": "148[8:9]-149[8:10]",
      "!type": "number",
      "!data": {
        "isConstructor": false,
        "type": "Number.prototype"
      }
    },
    "tagfile": "__DIR__/phantom_object.js"
  }
]
```
```ctags
mod	__DIR__/phantom_object.js	/mod/;"	v	lineno:1
func	__DIR__/phantom_object.js	/func/;"	f	lineno:3	namespace:mod	type:number function()
otherMod	__DIR__/phantom_object.js	/otherMod/;"	v	lineno:7
c	__DIR__/phantom_object.js	/c/;"	v	lineno:9	namespace:otherMod	type:number
```
