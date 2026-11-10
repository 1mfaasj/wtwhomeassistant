# WTW / Comfoair ventilation Lovelace card

A custom Lovelace card for WTW / ComfoAir ventilation systems.

## Features

- Inline SVG airflow visualization
- Dynamic airflow colors based on temperatures
- Safe fallbacks for unavailable entities
- Configurable entity names

## Installation with HACS

1. Install this repository as a custom HACS repository, and Dashboard type.
2. Now the 'Comfoair ventilation Lovelace card' becomes visible in HACS, click Download.
3. Restart Home Assistant if needed.
4. Add the lovelace card to your dashboard.

## Basic configuration

```yaml
type: custom:comfoair-card
entity: climate.comfoair
```

## Full configuration

All `entities` are optional; only override the ones whose entity id differs from the default.

```yaml
type: custom:comfoair-card
entity: climate.comfoair
title: Ventilatie
entities:
  outside_temperature: sensor.comfoair_outside_temperature
  intake_fan_rpm: sensor.comfoair_intake_fan_rpm
  exhaust_temperature: sensor.comfoair_exhaust_temperature
  exhaust_fan_rpm: sensor.comfoair_exhaust_fan_rpm
  return_temperature: sensor.comfoair_return_temperature
  return_air_level: sensor.comfoair_return_air_level
  supply_temperature: sensor.comfoair_supply_temperature
  supply_air_level: sensor.comfoair_supply_air_level
  filter_status: sensor.comfoair_filter_status
  supply_fan_active: binary_sensor.comfoair_supply_fan_active
  bypass_open: binary_sensor.comfoair_bypass_open
  preheating_state: binary_sensor.comfoair_preheating_state
  summer_mode: binary_sensor.comfoair_summer_mode
```

Tapping a temperature or a status icon opens the more-info dialog of that entity.
