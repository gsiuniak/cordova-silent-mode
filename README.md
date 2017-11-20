## Cordova Silent Mode

Forked from https://github.com/khevamann/cordova-silent-mode

This plugin determines is an iOS device is on silent mode or not.

## Installation

```bash
cordova plugin add https://github.com/gsiuniak/cordova-silent-mode
```

## Usage

```js
// Must be initialized before you wish to start observing changes //
SilentMode.init();

// Function with callbacks to determine whether or not device is muted - Will only run ONCE //
SilentMode.isMuted(
  function onMuted() { 
    console.log('Device ringer is OFF'); 
  }, 
  function onUnmuted() {  
    console.log('Device ringer is ON'); 
  });
```

## Supported Platforms

- iOS
