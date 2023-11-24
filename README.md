# Xenia Espresso Home Assistant
## Overview
This integration adds an on/off switch for the Xenia Espresso Machine and collects some sensors.

## Installation
Best would be to use the Visual Studio Code Server add-on for configuration.

1. Create a config/integrations directory if it does not already exist.
2. Copy the xenia-expresso.yaml file to config/integrations
3. Change the URL to the Name/IP of your Xenia IP Address in xenia-expresso.yaml (Line 14)
4. Include "xenia-espresso.yaml" by adding the following lines to your "configuration.yaml":

```yaml
homeassistant:
  packages: !include_dir_named integrations
```

Do not forget to check your configuration (Developer Tools --> hit "check configuration" and restart: it won't work without a restart!)

After the restart, some new sensors should be available. E.g., check for "sensor.xenia_status".
With the switch "switch.xenia" you can switch it on and off

## Contribution/Credits
This is based on the work of LagaV / Board Member of Kaffee-Netz - with some modifications
See Post: https://www.kaffee-netz.de/threads/xenia-dbl-schnittstellen-apis-fuer-home-automation-und-apps.151641/#post-2241348