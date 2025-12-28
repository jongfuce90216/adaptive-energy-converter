# Adaptive Energy Converter

An op-amp based voltage-matching circuit for solar/wind energy conversion to higher voltage battery.

## Problem Statement

Solar panels and wind turbines produce variable DC voltages depending on environmental conditions. To charge a higher voltage battery efficiently, the input voltage must be boosted and regulated to match the battery voltage. Traditional DC-DC converters may not optimally track the maximum power point while maintaining voltage matching.

This circuit uses an operational amplifier (op-amp) control loop to adjust the output voltage of a boost converter stage, ensuring that the converter's output matches the battery voltage over a wide input voltage range.

## System Block Diagram

```
[Solar Panel / Wind Turbine]  
        |  
        V  
[Voltage Sensing & Conditioning]  
        |  
        V  
[Op‑Amp Controller] → [PWM Driver] → [Boost Converter]  
        |  
        V  
[Battery Voltage Sensing]  
        |  
        V  
[Microcontroller (optional feedback)]  
        |  
        V  
[Higher Voltage Battery]
```

## Features

- **Wide input voltage range**: 5 V to 30 V DC (configurable)
- **Op‑amp based analog control**: Fast response, no software latency
- **Microcontroller interface**: For setpoint adjustment, monitoring and logging
- **Adjustable output voltage**: Matches battery voltage from 12 V to 48 V
- **Over‑current and over‑voltage protection** (optional)
- **Open‑source hardware & firmware**: Fully documented for replication

## Status

*Project is currently in development. The repository contains work‑in‑progress design files, firmware, and documentation.*

## Getting Started

Once the project is complete, this section will link to the assembly guide, schematic, and firmware.

## License

This project is licensed under the MIT License – see the LICENSE file for details.