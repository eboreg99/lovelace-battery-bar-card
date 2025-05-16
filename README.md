# 🔋 Battery Bar Card for Home Assistant

A customizable Lovelace card to display battery levels, supporting dynamic min/max values via entity or config.

## Installation via HACS

1. Add this repo as a custom repository in HACS:
   - URL: `https://github.com/eboreg99/battery-bar-card`
   - Type: Lovelace

2. Install the card via HACS.
3. Add the resource manually if needed:
   ```yaml
   url: /hacsfiles/battery-bar-card/battery-bar-card.js
   type: module
   ```

## Example Usage

```yaml
type: custom:battery-bar-card
entity: sensor.battery_level
max_entity: sensor.battery_max     # or use fixed_max: 100
min: 0
```

## Features

- Works in both `card` and `entity-row` mode
- Dynamic maximum from another entity
- Configurable fixed min/max
- Inline usage in entities card
