# Search Text Plugin for Notable
**Search Text Plugin for Notable** is a simple JS script for the  [Notable](https://github.com/notable/notable) application that allows you to find a search phrase in the current document.

![Image](https://raw.githubusercontent.com/DevTomek-pl/Search-Text-Plugin-for-Notable/master/readme/screen.png)

## Installation
Run the [Notable](https://notable.md) application and enable the Developer Tools `Help ->  Toggle Developer Tools`. 
Then switch to the `Console` tab and run one of the following scripts. (JS script should be executed each time the application is started)
          
#### Load from remote source (recommended)
```javascript
(async function () {
  let response = await fetch('https://raw.githubusercontent.com/DevTomek-pl/Search-Text-Plugin-for-Notable/master/search-text-plugin-for-notable.js');
  let script = await response.text();
  eval(script);
})();
```

#### Load from local source (optional)
```javascript
var script = document.createElement('script'); 
script.src = 'file:///{PATH_TO_PLUGIN}/search-text-plugin-for-notable.js'; 
document.body.appendChild(script);     
```  

## Shortcuts
* `Enter` - find next

## Related
* [markjs.io](https://markjs.io) - JavaScript keyword highlighter. Search term highlighting intended for every use case. Can be used with plain JavaScript or as jQuery plugin.


