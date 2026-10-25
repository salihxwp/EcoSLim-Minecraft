# EcoSim

EcoSim is an early-stage Minecraft mod project exploring a regional ecosystem simulation. Its goal is to model how wildlife populations, vegetation, habitat conditions, and predator-prey relationships could change over time.

> **Development prototype:** The current release does not yet connect the simulation to Minecraft worlds. It does not add visible animals, change in-game vegetation, or provide ecosystem gameplay.

## Project status

The project currently contains:

- A shared Java module with initial habitat, species, population, and simulation models.
- Unit tests for selected simulation behaviors.
- An initial Fabric entrypoint scaffold for Minecraft 1.21.1.

The Fabric entrypoint is not a complete gameplay integration. NeoForge is an unverified development scaffold, and Forge is not currently supported.

## Planned features

EcoSim is intended to grow toward:

- Regional habitat and vegetation tracking.
- Aggregate wildlife populations.
- Grazing and vegetation recovery.
- Data-driven predator-prey relationships.
- Habitat suitability based on environmental conditions.
- Periodic, performance-conscious simulation updates.
- Persistent ecosystem data saved with each world.
- Loader-specific integrations that share the same simulation core.

These are project goals, not features available in the current prototype.

## Compatibility

| Component | Status |
| --- | --- |
| Minecraft | 1.21.1 target |
| Java | 21 |
| Fabric | Initial scaffold; not yet connected to gameplay |
| NeoForge | Unverified scaffold |
| Forge | Not currently supported |

## Building

The project uses Gradle. With Java 21 and Gradle installed, run these commands from the repository root:

```bash
gradle :ecosim-common:test
gradle :ecosim-fabric:build
