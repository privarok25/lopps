# Loop Practice

A clean, independent Geode mod project for Geometry Dash 2.2081 / Geode SDK 5.11.2.

## Current scaffold (v0.1.0)
- Separate mod ID: `privarskii.looppractice`.
- Separate project and source tree; no Predictive Input Buffer code or behavior is included.
- Build configuration follows the supplied Geode project template.

## Planned implementation
1. In-game segment editor (start/end percentage).
2. Loop controller with explicit attempt states.
3. Streak, best streak, and death counter.
4. Configurable restart delay and countdown.

The percentage rewind mechanism is deliberately not implemented in this scaffold. A reliable rewind must restore level/player state, not merely teleport the player, because portals, triggers, dual mode, gravity, speed, and camera state can affect the result. This needs dedicated implementation and in-game validation before being advertised as functional.

## Build
Set `GEODE_SDK` to your Geode SDK directory, then configure/build with CMake as for a standard Geode mod.
