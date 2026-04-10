# Protocol Registry: System Nerves

To build a robust local system, resources are categorized by their complexity.

## Tier 1: Foundation Protocols
Resources for establishing the core messaging network.
* Mosquitto MQTT Broker Manual
* Tailscale Local-Remote Access

## Tier 2: Device Bridges
Tools that turns physical radio signals into network data.

### Featured Resource: Zigbee2MQTT Documentation
* **URL:** https://www.zigbee2mqtt.io
* **Definition & Purpose:** Zigbee2MQTT is an open-source bridge that turns Zigbee radio signals into MQTT messages, giving users local control of over 3,000 devices without the need for branded hubs. 
* **Value & Instruction:** For the specialist, this resource provides the "Device Database", which is important for making sure hardware will be compatible before purchase. To use it efficiently, navigate to the "Supported Devices" section and filter by "Exposes" to identify which specific sensors (like temperature or occupancy) can be used locally. Following the initial "Getting Started" configuration allows users to bypass "cloud-lock" and achieve sub-100ms response times.

## Tier 3: Custom Firmware
Tools for sending custom code to microcontrollers.
* ESPHome YAML Reference

[Return to Home](index.html)
