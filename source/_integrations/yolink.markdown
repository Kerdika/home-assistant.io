---
title: YoLink
description: Instructions on how to integrate YoLink Devices into Home Assistant.
ha_category:
  - Binary Sensor
  - Climate
  - Lock
  - Sensor
  - Siren
  - Switch
ha_release: 2022.6
ha_iot_class: Cloud Push
ha_config_flow: true
ha_codeowners:
  - '@matrixd2'
ha_domain: yolink
ha_platforms:
  - binary_sensor
  - climate
  - lock
  - sensor
  - siren
  - switch
ha_integration_type: integration
---

Integrates [YoLink](https://www.yosmart.com/) Devices into Home Assistant.

{% include integrations/config_flow.md %}

{% details "Using custom application credentials" %}
Home Assistant will use account linking provided by Nabu Casa for authenticating with YoLink, this service is provided for free and does not require a Nabu Casa subscription. The steps below are thus not required.
If you want to use separate credentials, please contact <service@yosmart.com> to obtain a `client_id` and `client_secret`. Then you can add your credentials via application credentials. Settings > Devices & Services > click the menu (three dots at the top right of the screen) and then **Application Credentials**. Enter your credentials in the pop-up window.
{% enddetails %}

The integration is tested and verified for the following devices from YoLink:

* YS6602/4 (outlet | plug)
* YS7103/4/5 (siren)
* YS7704 (door sensor)
* YS7804/5 (motion sensor)
* YS7903/4 (leak sensor)
* YS8003 (temperature/humidity sensor)
* YS7201 (vibration sensor)
* YS7607 (lock)
* YS4909 (valve controller)
* YS5705 (switch)
* YS7A01 (CO & Smoke Sensor)
* YS4002 (Thermostat)
