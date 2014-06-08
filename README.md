PinDialog
=========

PhoneGap numeric password dialog plugin for Android and iOS. Forked from https://github.com/apache/cordova-plugin-dialogs.git

Installation:

```cordova plugin add https://github.com/Paldom/PinDialog.git```
or
```phonegap local plugin add https://github.com/Paldom/PinDialog.git```

Usage:

    // Show pin dialog
    window.plugins.pinDialog.prompt("message", callback, "title", ["OK","Cancel"]);

Callback:

    function callback(results)
    {
        if(results.buttonIndex == 1)
        {
            // OK clicked, show input value
            alert(results.input1);
        }
        if(results.buttonIndex == 2)
        {
            // Cancel clicked
            alert("Cancel");
        }
    };
