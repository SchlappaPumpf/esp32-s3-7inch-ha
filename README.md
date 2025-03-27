# esp32-s3-7inch-ha
Just a test :)

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
    url: https://github.com/jtenniswood/esphome-lvgl/
    files: [device/esp32-s3-touch-lcd-7.yaml,
            addon/time.yaml,
            addon/backlight.yaml,
            addon/network.yaml,
            assets/fonts.yaml,
            assets/icons.yaml,
            assets/images.yaml,
            theme/button.yaml,
            office/sensors.yaml,
            office/lvgl.yaml]
    refresh: 1sec
```
