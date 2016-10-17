# Getting started with Arduino or NodeMCU development

Fiddeling with Arduino to get started.

Install an editor like Atom:
* https://atom.io/

Install PlatformIO:
* http://docs.platformio.org/en/stable/installation.html

Install drivers for NodeMCU:
* [Driver page](https://www.silabs.com/products/mcu/Pages/USBtoUARTBridgeVCPDrivers.aspx)
    * [Mac OS X](http://www.silabs.com/Support%20Documents/Software/Mac_OSX_VCP_Driver.zip)
    * [Windows](http://www.silabs.com/Support%20Documents/Software/CP210x_Windows_Drivers.zip)
    * [Linux](http://www.silabs.com/Support%20Documents/Software/Linux_3.x.x_VCP_Driver_Source.zip)


# Start a new project with Arduino Uno

Init project with PlatformIO:
```bash
$ mkdir Arduino-hello-world/
$ cd Arduino-hello-world/
$ platformio init --board uno
```

_Start developing :)_

Upload to controller:
```bash
$ platformio run -e uno -t upload
```

Show device monitor:
```bash
$ platformio device monitor
```


# Start a new project with NodeMCU

Install drivers for NodeMCU
https://www.silabs.com/products/mcu/Pages/USBtoUARTBridgeVCPDrivers.aspx

Init project with PlatformIO
```bash
$ cd NodeMCU-hello-world/
$ platformio init --board nodemcuv2
```

_Start developing :)_

Upload to controller and show device monitor:
```bash
$ pio run -e nodemcuv2 -t upload && pio serialports monitor -b 115200
```

Upload to controller:
```bash
$ platformio run -e nodemcuv2 -t upload
```

Show device monitor:
```bash
$ platformio serialports monitor -b 115200
```

# Other resources

* https://www.losant.com/blog/getting-started-with-platformio-esp8266-nodemcu
