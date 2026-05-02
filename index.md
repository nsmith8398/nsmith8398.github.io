# Local-First Smart Home Architecture

Welcome to the System Design Guide. I built this resource for fellow engineering students, developers, and hobbyists who want to build a smart home that doesn't rely on the cloud. 

If a manufacturer's server goes offline, your house shouldn't break. This guide provides the tools to build a private, fast system from the ground up.

## Guide Overview
* **Scope:** Covers local hubs, mesh networking (Zigbee/Thread), and local-only protocols. If you've taken any process control classes, this is basically just setting up small-scale control loops for your house.
* **Audience:** Engineering students and DIYers looking to build local, cloud-free systems.
* **Prerequisites:** Basic understanding of IP networking and microcontrollers (like a Raspberry Pi or ESP32).
* **Organization:** Starts with the central hub and works down to specific communication protocols.

## Tips for Using this Guide
* Use the links below to jump to specific tools.
* These resources focus on the actual code and configuration, not basic consumer tutorials. Always check the hardware compatibility lists and YAML examples first.

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
