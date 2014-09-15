<!--- Alauddin Ansari --->

# com.alauddin.cordova.deviceinfo

This plugin provides information about the device's Hardware and software.

## Cordova Version
    This plugin is tested on cordova version: 3.5.0

## Installation
    cordova plugin add https://github.com/AlauddinTheWonder/DeviceInfo-Cordova-Plugin.git

## Supported Platforms
    - Android

## Methods
    - navigator.deviceinfo.getInfo

### Parameters
    - __callBackSuccess__: The callback that is passed the device info.
    - __callBackError__: _(Optional)_ The callback that executes if an error occurs.

### Example
    navigator.deviceinfo.getInfo(onSuccess, onError);
    
    // onSuccess Callback receives a Device Info object
    //
    function onSuccess(info) {
        alert("Phone Number: "  + info.msisdn + "\n" +
          "IMEI Number: "       + info.imei + "\n" +
          "Sim Operator: "      + info.operator + "\n" +
          "Sim Operator Name: " + info.operator_name + "\n" +
          "Country ISO: "       + info.country_iso + "\n" +
          "Roaming: "           + info.roaming + "\n" +
          "Device Model: "      + info.model + "\n" +
          "Device Manufacturer: "   + info.manufacturer + "\n" +
          "Phone Type: "        + info.phone_type + "\n" +
          "IP Address: "        + info.ip + "\n" +
          "Connection Type: "   + info.connection_type
        );
    };

    // onError Callback receives a DeviceInfoError object
    //
    function onError(error) {
        alert('message: ' + error);
    }




