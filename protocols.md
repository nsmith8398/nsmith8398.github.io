# Protocol Registry: System Nerves

To build a solid local system, I've broken down the resources by what they do.

## Tier 1: Foundation Protocols
Tools for setting up your core network and secure remote access.

### Mosquitto MQTT Broker Documentation
* **URL:** [https://mosquitto.org/documentation/](https://mosquitto.org/documentation/)
* **Definition, Purpose, and Scope:** Eclipse Mosquitto is an open-source message broker for the MQTT protocol. It's the main system that sends data from your sensors to your main hub. The scope of this documentation covers command-line setup, broker configuration, and authentication for security.
* **Value and Instruction:** A local broker is required if you want your devices to talk to each other instantly without going through the cloud. This documentation gives you the exact terminal commands you need. *Tip:* Jump straight to the `mosquitto.conf` section to see how to set up usernames and passwords so your local network stays secure.

### Tailscale Knowledge Base
* **URL:** [https://tailscale.com/kb/](https://tailscale.com/kb/)
* **Definition, Purpose, and Scope:** Tailscale is a zero-config VPN built on WireGuard. Its docs explain how to create a private network between your phone and your home server. The scope covers installation, subnet routing, and access control.
* **Value and Instruction:** The hardest part of a cloud-free smart home is controlling it when you aren't home. Tailscale fixes this without making you open dangerous ports on your router. Read the "Subnet Routers" guide to learn how to access your whole home network from your phone while traveling.

## Tier 2: Device Bridges
Software that translates physical radio signals into network data.

### Zigbee2MQTT Documentation
* **URL:** [https://www.zigbee2mqtt.io](https://www.zigbee2mqtt.io)
* **Definition, Purpose, and Scope:** Zigbee2MQTT is an open-source bridge that grabs Zigbee radio signals and turns them into MQTT messages, letting you use over 3,000 devices locally without their hubs. The scope includes the supported device database, filtering options, and the initial setup guide.
* **Value and Instruction:** This is your go-to reference for making sure a sensor will work before you buy it. Go to the "Supported Devices" section and filter by "Exposes" to see exactly what data (like temperature or motion) a device can send locally. Using this tool gets rid of cloud delays and gives you instant response times.

### CSA Matter Specification
* **URL:** [https://csa-iot.org/developer-resource/specifications-download-request/](https://csa-iot.org/developer-resource/specifications-download-request/)
* **Definition, Purpose, and Scope:** This is the official technical standard from the Connectivity Standards Alliance (CSA) for Matter. It's the shared language that lets different brands of smart devices work together locally. The scope talks about standard device data clusters and local connection rules for Thread and Wi-Fi.
* **Value and Instruction:** If you are building IoT tools, you need this to understand how to connect devices without downloading ten different apps. Check the "Device Library" section to see exactly what data is required to run specific devices, like smart locks or thermostats.

## Tier 3: Custom Firmware
Tools for writing custom code to your own microcontrollers.

### ESPHome YAML Reference
* **URL:** [https://esphome.io/](https://esphome.io/)
* **Definition, Purpose, and Scope:** ESPHome lets you program microcontrollers (like ESP8266 and ESP32 boards) using simple YAML files instead of writing raw code. The reference guide is the manual for putting this custom firmware together. The scope covers syntax formatting with YAML and integration examples for different sensors.
* **Value and Instruction:** This is perfect if you want to solder your own cheap, custom sensors (like sticking a temperature, humidity, and motion sensor in one box). *Tip:* Skip the deep C++ sections entirely. Just use the "Cookbook" section to find pre-written YAML blocks that you can copy and paste into your own project.

<footer>
  <div class="footer-nav">
    <span><a href="hub.html">← Previous: The Core Hub</a></span>
    <span><a href="index.html">Return to Home ↑</a></span>
  </div>
</footer>
