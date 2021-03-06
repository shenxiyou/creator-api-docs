## `Pipeline.Downloader` Class



Module: [cc](../modules/cc.md)
Parent Module: [cc](../modules/cc.md)


The downloader pipe, it can download several types of files:
1. Text
2. Image
3. Script
4. Audio
5. Assets
All unknown type will be downloaded as plain text.
You can pass custom supported types in the constructor.


### Index



##### Methods

  - [`constructor`](#constructor) Constructor of Downloader, you can pass custom supported types.
  - [`addHandlers`](#addhandlers) Add custom supported types handler or modify existing type handler.
  - [`loadSubpackage`](#loadsubpackage) Load subpackage with name.



### Details




<!-- Method Block -->
#### Methods


##### constructor

Constructor of Downloader, you can pass custom supported types.

| meta | description |
|------|-------------|
| Defined in | [cocos2d/core/load-pipeline/downloader.js:270](https://github.com/cocos-creator/engine/blob/d6ec4c03aa86f40af14d21ef9f059fed5e540c58/cocos2d/core/load-pipeline/downloader.js#L270) |

###### Parameters
- `extMap` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> Custom supported types with corresponded handler

##### Examples

```js
var downloader = new Downloader({
     // This will match all url with `.scene` extension or all url with `scene` type
     'scene' : function (url, callback) {}
 });
```

##### addHandlers

Add custom supported types handler or modify existing type handler.

| meta | description |
|------|-------------|
| Defined in | [cocos2d/core/load-pipeline/downloader.js:295](https://github.com/cocos-creator/engine/blob/d6ec4c03aa86f40af14d21ef9f059fed5e540c58/cocos2d/core/load-pipeline/downloader.js#L295) |

###### Parameters
- `extMap` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> Custom supported types with corresponded handler


##### loadSubpackage

Load subpackage with name.

| meta | description |
|------|-------------|
| Defined in | [cocos2d/core/load-pipeline/downloader.js:353](https://github.com/cocos-creator/engine/blob/d6ec4c03aa86f40af14d21ef9f059fed5e540c58/cocos2d/core/load-pipeline/downloader.js#L353) |

###### Parameters
- `name` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> Subpackage name
- `completeCallback` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Function" class="crosslink external" target="_blank">Function</a> Callback invoked when subpackage loaded
	- `error` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Error" class="crosslink external" target="_blank">Error</a> error information



