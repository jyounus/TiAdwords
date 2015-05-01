# TiAdwords


AdWords SDK for Titanium. 64bit ready. Download compiled module from the dist folder. 


Just a quick wrapper for the latest Google AdWords SDK for iOS (GoogleConversionTrackingSDK-iOS-3.2.0).

There is an [existing module](https://github.com/jkotchoff/adwords_conversion_tracking_titanium_module) on Github but it's outdated and using a depricated SDK. For some reasons, I had issues updating it to the latest version, so I decided to create a brand new module from scratch instead of wasting my time any further.


===

### Usage

Add it to your tiapp.xml:

`<module platform="iphone">co.uk.devpulse.tiadwords</module>`
    

In your controller, call it like this:

    var TiAdwords = require("co.uk.devpulse.tiadwords");
    TiAdwords.sendRequest({
        conversionId:"conversionId here",
        label:"label here",
        value:"value here",
        isRepeatable:true
    });
    
    
All properties are required otherwise it won't work.