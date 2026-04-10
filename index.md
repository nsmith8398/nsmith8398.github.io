# Local-First Smart Home Architecture

Welcome to the system design guide for building a cloud-independent smart home.

### About This Guide
* **The Problem:** Cloud-dependent smart devices have latency issues, privacy risks, and can get "bricked" if the company shuts down.
* **Audience:** This is for prosumers, engineering students, and IoT developers.
* **Scope:** Covers the system architecture for local hubs, mesh networking (Zigbee/Thread), and custom firmware.

### Before You Start
* **Assumed Knowledge:** You should understand basic IP networking and have some baseline experience with microcontrollers (like a Raspberry Pi or ESP32). 

### Navigating the Site
This guide is organized top-down: starting with the main hub and working down to the specific device protocols. 

**Tips for use:** Use the links below to jump to the specific architectural layer you need. Focus on the provided documentation links for configuration steps.

---

### Table of Contents
* **[The Core Hub](hub.html)**: Local operating systems and coordinators.
* **[Protocol Registry](protocols.html)**: Communication standards, bridges, and firmware.
