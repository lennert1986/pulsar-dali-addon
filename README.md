# Pulsar DALI Home Assistant App

Home Assistant App repository for the Glamox / ES-SYSTEM Pulsar CM4 DALI controller.

## Install

In Home Assistant OS / Supervised:

1. Open **Settings → Apps → App store**.
2. Open **Repositories** from the menu.
3. Add:

   `https://github.com/lennert1986/pulsar-dali-addon`

4. Install **Pulsar DALI Control**.

## Hardware mapping

- DALI 1: `/dev/ttyAMA3`
- DALI 2: `/dev/ttyAMA4`
- DALI 3: `/dev/ttyAMA5`
- Front-panel LEDs: MCP23017 on I²C bus 1, address `0x20`

The App contains commissioning, address repair, groups, scenes, DALI-2 inputs, secure remote API, and central management.
