# Local-First Smart Home Architecture: System Design Guide

## The Problem Statement
The cloud is just someone else's computer. Modern consumer IoT devices suffer from "cloud-dependency" and "vendor lock-in." When a cloud company goes bankrupt or shuts down servers, devices are frequently "bricked" and rendered useless. Furthermore, sending home data to external servers introduces significant security risks and latency. This guide helps specialists solve this challenge by integrating fragmented, open-source tools into a cohesive, internet-independent system.

## Who the Guide is For (Audience & Purpose)
This guide is designed for **"prosumer" specialists**, including engineering students and IoT developers, who are highly motivated by a desire for privacy, zero-latency, and total ownership of their home hardware. Its purpose is to provide a curated technical masterlist of resources that allow these specialists to build a high-performance system from the ground up, without relying on proprietary, cloud-based consumer hubs.

## What's in the Guide (Scope)
This guide addresses the system architecture and implementation of local-first smart homes. It focuses on the technical layers required to build an automation ecosystem that operates independently of third-party cloud servers, specifically covering local hubs and mesh networking protocols like Zigbee and Thread.

## What the Guide Assumes Users Know
Readers should understand basic IP networking and have introductory experience with microcontrollers (such as the Raspberry Pi or ESP32). The guide builds on this foundational knowledge while providing necessary background information on Network Layers and how local coordinators communicate with sensors via non-Wi-Fi frequencies.

## How the Guide is Organized
Because this guide is built for specialists, it is organized **deductively**. It moves from the "Brain" of the system (the central hub) down to the "Nerves" (the edge sensors and communication protocols). 

## Tips for Using this Guide
* **Use the Navigation:** Rely on the two-level Table of Contents below to jump directly to the specific architectural layer you are currently designing.
* **Focus on Configuration:** The resources linked in this guide use efficient, technical language focused on deployment and configuration. Do not expect basic consumer tutorials; instead, look for hardware interoperability warnings and YAML examples.

---

## Site Navigation (Table of Contents)

### 1. [The Core Hub](hub.html)
* Central coordinators and local operating systems.

### 2. [Protocol Registry](protocols.html)
* **Tier 1:** Foundation Protocols
* **Tier 2:** Device Bridges
* **Tier 3:** Custom Firmware
