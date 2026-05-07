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
- Traction control
- ABS
- Reverser handling
- Real-time drivetrain state processing

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

## Project Structure

```text
stormworks-train-drivetrain/
├── README.md
├── vehicle/
│   └── drivetrain_controller.xml
├── lua/
│   ├── drivetrain_source.lua
│   └── drivetrain_compact.lua
├── images/
└── docs/
```

---

## Files

### `drivetrain_controller.xml`
Full Stormworks microcontroller containing:
- Logic connections
- System interfaces
- Embedded Lua script
- Control architecture

### `drivetrain_source.lua`
Readable and documented source version of the drivetrain controller.

### `drivetrain_compact.lua`
Optimized in-game version designed around Stormworks character limits.

---

## Screenshots

_Add screenshots here_

Suggested screenshots:
- Driver desk
- Locomotive control interface
- Drivetrain diagnostics
- Logic overview
- TCP integration example

Example image markdown:

```md
![Driver Desk](images/driver_desk.png)
```

---

## Future Improvements

Planned or possible future development:
- Expanded train telemetry
- Advanced traction management
- Multi-unit synchronization
- Configurable control profiles
- Additional TCP interoperability features

---

## License

MIT License
