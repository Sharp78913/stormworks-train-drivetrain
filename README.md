# Stormworks Train Drivetrain

A custom locomotive drivetrain and braking control system developed for Stormworks.

This project was designed for advanced train simulation and control, with compatibility considerations for the SRC-TCP train communication ecosystem while remaining an independent controller architecture.

The controller focuses on:
- Working within a large train consist
- Real-time drivetrain management
- Modular train control logic
- Driver interface integration
- Multi-cab operation
- Optimized Stormworks Lua execution

---

## Relationship to TCP

I am a contributor/developer within the TCP ecosystem:

https://github.com/SRC-org/TCP

This drivetrain controller is currently an independent project and is not yet part of the official TCP framework.

The system was developed with interoperability and modular vehicle systems in mind, including:
- Shared train interfaces
- Distributed subsystem control
- Multi-unit compatibility
- Expandable architecture

---

## Features

### Drivetrain Control
- Throttle management for a target speed or direct throttle from the driver
- ABS
- Reverser handling
- Real-time drivetrain state processing

### Traction Control
- Predictive method, Based off wheel speed sensor.
- Corrective method, Based off when slip is detected

### Braking Systems
- Dynamic braking logic
- Independent brake handling
- Automatic state management
- Driver feedback integration

### Vehicle Systems
- Multi-cab compatibility
- Modular subsystem architecture
- TCP-oriented integration design
- Real-time control updates

### UI / Driver Integration
- Driver desk integration
- Control feedback systems
- Status monitoring
- Optimized display interaction

---

## Technical Highlights

This project was developed around several Stormworks constraints and engineering considerations:

- Character-limited Lua environments
- Real-time vehicle state processing
- Driver interface support
- Modular train system integration

The compact in-game Lua implementation uses:
- Shortened variable naming
- Function aliasing
- Reduced whitespace

to remain within Stormworks microcontroller limitations.

---

## Future Improvements

Planned or possible future development:
- More traction methods for different train setups
- Multi-unit synchronization
- Configurable control profiles
- Additional TCP interoperability features

---

## License

MIT License
