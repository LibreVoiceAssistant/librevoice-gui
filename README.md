# LibreVoice GUI Service

GUI service for GUI clients based on the LibreVoice GUI Framework.

# Configuration

under mycroft.conf

```javascript
{
  "gui": {
    // Override: SYSTEM (set by specific enclosures)
    // Uncomment or add "idle_display_skill" to set initial homescreen
    // "idle_display_skill": "skill-ovos-homescreen.openvoiceos",

    // Extensions provide additional GUI platform support for specific devices
    // Currently supported devices: smartspeaker, bigscreen or generic
    "extension": "generic",

    // Generic extension can additionaly provide homescreen functionality
    // homescreen support is disabled by default for generic extension
    "generic": {
        "homescreen_supported": false
    }
  },
  
  // The GUI messagebus websocket.  Once port is created per connected GUI
  "gui_websocket": {
    "host": "0.0.0.0",
    "base_port": 18181,
    "route": "/gui",
    "ssl": false
  }
}
```
