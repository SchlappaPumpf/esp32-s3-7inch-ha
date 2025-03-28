# esp32-s3-7inch-ha
Just a test :)

These snippets are mostly copied from other repositories - I'll try to do my very best to mention them...

add to yaml-file:


```yaml
substitutions:
  name: "test"
  friendly_name: "test"
  room: "Wohnzimmer"

# Wifi Setup
wifi:
  ssid: !secret wifi_ssid
  password: !secret wifi_password

# Packages
packages:
  setup:
    url: https://github.com/SchlappaPumpf/esp32-s3-7inch-ha/
    files: [device/test/device_wohnzimmer.yaml,
            device/test/dht22_wohnzimmer.yaml]
    refresh: 1sec
```
