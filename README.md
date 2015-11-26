# node-ssdp-js

## Usage
```javascript
var Browser = require("ssdp-js");
var browser = new Browser();
browser.start(); // by default, ssdp-js would poll ssdp every 5 seconds

browser.onDevice(function(device) {
  device.onError(function(err) { console.error("DNLA device error", err) });

  console.log("DLNA device ", device.name, device.host);
  //var MediaRendererClient = require("upnp-mediarenderer-client");
  //var client = new MediaRendererClient(device.xml);
});

```
