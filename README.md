# rainbird2
Home assistant component for second rainbird controller

It is just a workaround to get second controller working

Usage: 
just add rainbird2 folder to custom_components folder in Home Assistant config directory: #config_dir#/custom_components/rainbird2


Sample home assistant config:


rainbird:
  - host: IP_ADDRESS_OF_MODULE
    password: YOUR_PASSWORD
    trigger_time: 6
    zones:
      1:
        friendly_name: My zone 1
        trigger_time:
          minutes: 6
      2:
        friendly_name: My zone 2
        trigger_time: 2
rainbird2:
  - host: IP_ADDRESS_OF_ANOTHER_MODULE
    password: YOUR_ANOTHER_PASSWORD
    trigger_time: 0:06
    zones:
      1:
        friendly_name: My zone 1
        trigger_time: 0:06
      2:
        friendly_name: My zone 2
        trigger_time: 0:05
