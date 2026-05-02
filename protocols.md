# Protocol Registry: System Nerves

To build a robust local system, resources are categorized by their complexity.

## Tier 1: Foundation Protocols
Resources for establishing the core messaging network and secure access.

### Mosquitto MQTT Broker Documentation
* **URL:** [https://mosquitto.org/documentation/](https://mosquitto.org/documentation/)
* **Definition, Purpose, and Scope:** Eclipse Mosquitto is an open-source message broker that handles the MQTT protocol. It acts as the central delivery system that passes messages between local sensors and the main hub. The scope of this documentation includes command-line syntax, broker configuration, and authentication setup.
* **Value and Instruction:** Because local smart homes rely on rapid device-to-device communication, a local broker is required to avoid sending data to the cloud. For developers, this documentation provides the exact command-line syntax needed to run the broker. A useful tip is to go straight to the `mosquitto.conf` section to learn how to set up username and password authentication, which keeps the local network secure.

### Tailscale Knowledge Base
* **URL:** [https://tailscale.com/kb/](https://tailscale.com/kb/)
* **Definition, Purpose, and Scope:** Tailscale is a zero-config VPN built on the WireGuard protocol. Its documentation explains how to create a secure, private network between remote devices and the local home network. The scope of this knowledge base covers installation protocols, subnet router configuration, and access control lists.
* **Value and Instruction:** One of the main challenges of a cloud-free smart home is securely controlling it while away from home. Tailscale solves this by providing remote access without requiring you to open vulnerable ports on your router. To use this efficiently, read the "Subnet Routers" guide to learn how to expose your entire home LAN to your phone when you are traveling.

## Tier 2: Device Bridges
Tools that turn physical radio signals into network data.

### Zigbee2MQTT Documentation
* **URL:** [https://www.zigbee2mqtt.io](https://www.zigbee2mqtt.io)
* **Definition, Purpose, and Scope:** Zigbee2MQTT is an open-source bridge that turns Zigbee radio signals into MQTT messages, giving users local control of over 3,000 devices without the need for branded hubs. The scope encompasses the device database, supported sensor filtering, and initial bridge configuration.
* **Value and Instruction:** For the specialist, this resource provides the "Device Database", which is important for making sure hardware will be compatible before purchase. To use it efficiently, navigate to the "Supported Devices" section and filter by "Exposes" to identify which specific sensors (like temperature or occupancy) can be used locally. Following the initial "Getting Started" configuration allows users to bypass "cloud-lock" and achieve sub-100ms response times.

### CSA Matter Specification
* **URL:** [https://csa-iot.org/developer-resource/specifications-download-request/](https://csa-iot.org/developer-resource/specifications-download-request/)
* **Definition, Purpose, and Scope:** This is the official technical registry provided by the Connectivity Standards Alliance (CSA) for the Matter protocol. It details the standardized language that allows different brands of smart devices to talk to each other locally. The scope details standard device clusters and local provisioning requirements via Thread or Wi-Fi.
* **Value and Instruction:** For an IoT developer, understanding these specifications is necessary for provisioning devices locally via Thread or Wi-Fi without downloading a vendor's specific app. When using this resource, check the "Device Library" section to understand exactly which data clusters are required for specific device types (like smart locks or thermostats).

## Tier 3: Custom Firmware
Tools for sending custom code to microcontrollers.

### ESPHome YAML Reference
* **URL:** [https://esphome.io/](https://esphome.io/)
* **Definition, Purpose, and Scope:** ESPHome is a system that lets you control microcontrollers (like ESP8266 and ESP32 boards) using simple YAML configuration files. The reference guide serves as a manual for compiling custom C++ firmware. The scope covers YAML syntax, custom C++ firmware compilation, and cookbook snippets for sensor integration.
* **Value and Instruction:** This is highly valuable for specialists who want to build their own custom sensors (like a combined temperature, humidity, and motion sensor) for a fraction of the cost of commercial products. To use this guide effectively, skip the deep technical C++ explanations and use the "Cookbook" section to find pre-written YAML snippets that you can copy and paste into your configuration.

<footer>
  <div class="footer-nav">
    <span><a href="hub.html">← Previous: The Core Hub</a></span>
    <span><a href="index.html">Return to Home ↑</a></span>
  </div>
</footer>
