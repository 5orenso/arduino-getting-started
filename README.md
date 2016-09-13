# arduino-getting-started

Fiddeling with Arduino to get started.

Install PlatformIO
```bash
$ sudo python -c "$(curl -fsSL https://raw.githubusercontent.com/platformio/platformio/master/scripts/get-platformio.py)"
```

Init project with PlatformIO
```bash
$ cd arduino-getting-started/
$ platformio init --board uno --board nodemcuv2
```

Upload to controller
```bash
$ platformio run -e uno -t upload
```

Show device monitor
```bash
$ platformio device monitor
```

