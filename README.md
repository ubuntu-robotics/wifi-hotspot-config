# wifi-hotspot-config
wifi hotspot configurator snap

[Install the snap from the Snap Store](https://snapcraft.io/wifi-hotspot-config).

Make sure to connect the `network-manager` interface:

```
snap connect wifi-hostspot-config:network-manager network-manager:service
```

The snap contains only one oneshot application.

The hotspot will be recreated at every boot or on install.

This snap has been tested on [Ubuntu Core 20](https://ubuntu.com/core).

## Configurations

The snap takes 3 configurations:
- `ssid`, the ssid of the hotspot to create. Default value: `Ubuntu Core Hotspot`
- `password`, the password if the hotspot to create. Default value: `0123456789`
- `wifi-interface`, the name of the wifi interface to use for the hotspot. Default value: `wlan0`

