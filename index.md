# Local-First Smart Home Architecture

Welcome to the System Design Guide. This resource is for developers, engineering students, and hobbyists looking to build a smart home that doesn't rely on the cloud. 

If a manufacturer's server goes offline, your house shouldn't stop working. This guide provides tools to build a private, zero-latency system from the ground up.

## Guide Overview
* **Scope:** Covers local hubs, mesh networking (Zigbee/Thread), and local-only protocols.
* **Audience:** Prosumers, engineering students, and IoT developers.
* **Prerequisites:** Basic understanding of IP networking and microcontrollers (like Raspberry Pi or ESP32).
* **Organization:** Deductive structure, moving from the central hub down to specific protocols and sensors.

## Tips for Using this Guide
* Use the navigation links below to jump to specific pages and resources.
* The linked resources focus on system configuration and code, rather than basic consumer tutorials. Look for hardware compatibility lists and YAML examples.

---

## Table of Contents

* **1. [The Core Hub](hub.html)** - Central coordinators and operating systems.
  * Home Assistant Core Documentation
* **2. [Protocol Registry](protocols.html)** - Communication standards and hardware bridges.
  * Tier 1: Foundation Protocols (Mosquitto MQTT, Tailscale)
  * Tier 2: Device Bridges (Zigbee2MQTT, CSA Matter Specs)
  * Tier 3: Custom Firmware (ESPHome)

<footer>
  <p style="text-align: center;">
    <em>Guide created for specialist-to-specialist communication. Last updated: May 2026</em>
  </p>
</footer>
