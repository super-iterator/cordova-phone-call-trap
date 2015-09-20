Cordova PhoneCall Trap with Caller Number 
=======================

This is a very practical extension to the original plugin, that allows you to receive incoming numbers, and decide accordingly what to do with them.


## Install

    $ cordova plugin add io.gvox.plugin.phonecalltrap


## Quick Example

    PhoneCallTrap.onCall(function(state) {
    alert("CHANGE STATE: " + state.state);

    switch (state.state) {
        case "RINGING":
            alert("Phone is ringing: " + state.number);
            break;
        case "OFFHOOK":
            alert("Phone is off-hook");
            break;

        case "IDLE":
            alert("Phone is idle");
            break;
        }
    });


## Supported platforms

- Android 2.3.3 or higher

## License

Cordova PhoneCall Trap is released under the [MIT License](http://www.opensource.org/licenses/MIT).
