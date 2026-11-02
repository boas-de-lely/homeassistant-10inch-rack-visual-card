# Home Assistant 10" Rack Visual Card

A custom Home Assistant dashboard card that recreates a compact 10-inch rack layout using SVG graphics and Bubble Card popups. It is designed to visually represent a small rack setup and provide quick access to status information for hardware, network traffic, and connected services.

## Overview

This project includes a single YAML configuration file that creates a detailed rack-style visual dashboard. The card uses a graphic background with clickable hotspots that open pop-up cards for the following sections:

- Home Assistant status
- Network traffic overview
- Access point traffic
- Proxmox / host monitoring
- Service-level panels such as Metro API, Pi-hole, and NAS-related status views

## Files

- [full layout.yaml](full layout.yaml) — the complete Lovelace card configuration
- [README.md](README.md) — project documentation

## Features

- SVG-based rack illustration with port mapping
- Clickable navigation areas for each rack section
- Pop-up views powered by Bubble Card
- Monitoring cards for CPU, RAM, storage, and networking
- Integration-ready placeholders for server and network entities
- Designed for a compact 10-inch dashboard layout

## Requirements

This dashboard depends on custom cards in Home Assistant, including:

- Bubble Card
- Mushroom Cards
- ApexCharts Card
- Masonry Layout
- Any custom cards referenced by the configuration for graphs and pop-ups

If you are using HACS, install the required cards before importing this configuration.

## Installation

1. Open your Home Assistant dashboard in the UI.
2. Go to the Lovelace dashboard editor.
3. Add a new card or use the YAML editor.
4. Copy the contents of [full layout.yaml](full layout.yaml) into a card or dashboard configuration that matches your existing setup.
5. Adjust your entity IDs to match your own Home Assistant installation.

## Customization

You may want to change these items:

- Entity IDs for sensors and devices
- Card titles and labels
- Colors and rack branding
- Which services or devices are exposed in the pop-up cards

The file is intentionally structured so that the visual layout and the popup content can be modified independently.

## Notes

- The YAML includes many entity references that are specific to the original setup. You will likely need to replace them with your own entity names.
- This is best used as a starting point or a visual inspiration rather than a drop-in dashboard for every Home Assistant instance.
- The SVG drawing is static, while the live data comes from the entities you connect to it.

## License

This project is intended for personal or home automation use. If you plan to reuse it publicly, adapt the content to match your own environment and naming conventions.

## Example use case

This design is ideal for monitoring:

- A small home lab rack
- A local network appliance stack
- A media server / hypervisor setup
- A compact dashboard for infrastructure status at a glance

If you want, I can also turn this into a cleaner version with:

- a more polished README
- installation steps for HACS and Lovelace
- a simplified version that is easier to customize
- a version with placeholder entity names for copy-paste use
