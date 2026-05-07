# Simulation Parameters

This file summarizes the main parameters used in the simulation examples.

## Geometric parameters

| Parameter | Description | Value |
|---|---|---|
| `L` | Segment length | 0.25 m |
| `r` | Effective tendon moment arm | 0.020 m |

## Motor--tendon parameters

| Parameter | Description | Value |
|---|---|---|
| `a` | Spool radius | 0.015 m |
| `N` | Gear ratio | 50 |
| `J` | Motor inertia | 4e-4 kg m² |
| `b` | Motor viscous friction | 2.2e-3 N m s/rad |
| `k` | Tendon--sheath stiffness | 100 N/m |
| `d` | Tendon--sheath damping | 0.5 N s/m |
| `l0` | Tendon rest length / pretension offset | 0 |

## Notes

The parameter `r` is interpreted as an effective tendon moment arm. It depends on the tendon routing geometry and may be refined through calibration or measured tendon-length variations.

The parameters `k` and `d` represent effective tendon--sheath stiffness and damping. They may be obtained from component data, calibration experiments, or simulation design assumptions.