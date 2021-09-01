# ArduinoSerialPnPExample

Based upon [IoT Plug and Play bridge](https://github.com/Azure/iot-plug-and-play-bridge) Arduino SerailPnP example at [here](https://github.com/Azure/iot-plug-and-play-bridge/tree/master/serialpnp/ArduinoExample).

**This is a work in progress**  
The overall aim here is to implement a PnP component that handles the [Grove Beginner Kit for Arduino](https://wiki.seeedstudio.com/Grove-Beginner-Kit-For-Arduino) functionality.

- Implements temeperature measurement with Grove BME280 Sensor.
- Implements some properties and commands but can't get these to work from Azure IoT Explorer.

# Config
- Has config.json is in repository in Config folder
  - Eg run with  .\pnpbridge_bin C:\Users\me\source\repos\ArduinoSerailPnPExample\Config\config.json
- Has schema file in Schema folder.
  - Eg in IoT Explorer from IOt Plug and Ply Components tab, [Configure], select Local folder and set to say, C:\Users\me\source\repos\ArduinoSerailPnPExample\Schema


## What works:

- Can send read and send the temperature to IoT Hub.
- Can view the received Telemetry in IoT Explorer.
- Can see the Interface, Writeable property, Commands in IoT Explorer.

## What doesn't work
 - In IoT Explorer - IoT Plug and Play 
   - No modeled Telemetry will show. Only the initial message that all is OK.,
   - Writeable property gets sent and brifge app logs its reception but nothing happens after that.
   - Commands fail
 
