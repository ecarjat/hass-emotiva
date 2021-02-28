![GitHub release (latest by date)](https://img.shields.io/github/v/release/ecarjat/hass-emotiva?style=for-the-badge) ![GitHub Release Date](https://img.shields.io/github/v/release/ecarjat/hass-emotiva?style=for-the-badge)

# Emotiva integration for Home Assistant
The emotiva integration identifies Emotiva devices on the network and adds them as entities in Home Asssitant

## Installation

### Install via HACS

The custom component will soon be available via

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)

### Manual Install

If you want to install the custom commponent manually, add the folder `emotiva/` to `YOUR_CONFIG_DIR/custom_components/`.

### Requirements
The component has only been tested with an XMC-1 so it might not work with other Emotiva devices.

### Configuration

Open the configuration file (`configuration.yaml`) and add the following
```yaml
media_player:
  - platform: emotiva
```
If an Emotiva devivce is detected on the network it will show up under entities with the name `media_player.[device_name]_[model_name]`
