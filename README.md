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
4. Restart Home Assistant if needed.
5. Add the lovelace card to your dashboard.

## Basic configuration

```yaml
type customcomfoair-card
entity climate.comfoair
``
