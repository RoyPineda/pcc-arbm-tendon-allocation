# Spatial RRPRRRRPRR DH Parametrization

This file provides the Denavit--Hartenberg (DH) parametrization of the spatial 10-link augmented rigid-body chain used for one 3D PCC segment.

## Augmented coordinates

For a spatial PCC segment, the reduced coordinates are

```math
q_i = [\phi_i,\ \theta_i]^\top ,
```
where $\phi_i$ is the bending-plane orientation and theta_i is the bending magnitude.

The corresponding augmented configuration is
```math
\xi_i = m_i(\phi_i, \theta_i)\in\mathbb{R}^{10},
```

For compactness, the main paper defines
```math
\beta(\theta_i)=\tfrac{\theta_i}{2} - \eta_i(\theta_i),
```

Then the curvature-to-ARBM mapping is

```math
m_i(\phi_i,\theta_i)= [\phi_i, \beta(\theta_i), b_i(\theta_i),\eta_i(\theta_i),-\phi_i,\phi_i,\eta_i(\theta_i),b_i(\theta_i), \beta(\theta_i),-\phi_i\,]^\top,
```

## DH table

<div align="center">

| Link | $\theta$ | $d$ | $a$ | $\alpha$ | $\mu$ |
|------|----------|-----|-----|----------|-------|
| 1 | $\xi_{10(i-1)+1}$ | $0$ | $0$ | $-\frac{\pi}{2}$ | $0$ |
| 2 | $\xi_{10(i-1)+2}$ | $0$ | $0$ | $+\frac{\pi}{2}$ | $0$ |
| 3 | $0$ | $\xi_{10(i-1)+3}$ | $0$ | $-\frac{\pi}{2}$ | $0$ |
| 4 | $\xi_{10(i-1)+4}$ | $0$ | $0$ | $+\frac{\pi}{2}$ | $0$ |
| 5 | $\xi_{10(i-1)+5}$ | $0$ | $0$ | $0$ | $\mu_i$ |
| 6 | $\xi_{10(i-1)+6}$ | $0$ | $0$ | $-\frac{\pi}{2}$ | $0$ |
| 7 | $\xi_{10(i-1)+7}$ | $0$ | $0$ | $+\frac{\pi}{2}$ | $0$ |
| 8 | $0$ | $\xi_{10(i-1)+8}$ | $0$ | $-\frac{\pi}{2}$ | $0$ |
| 9 | $\xi_{10(i-1)+9}$ | $0$ | $0$ | $+\frac{\pi}{2}$ | $0$ |
| 10 | $\xi_{10(i-1)+10}$ | $0$ | $0$ | $0$ | $0$ |

</div>

## Description

The RRPRRRRPRR chain is used as an augmented rigid-body representation of a spatial constant-curvature segment. The chain is constrained by the mapping $\xi_i = m_i(\phi_i, \theta_i)$ so that it reproduces the geometry of the corresponding 3D PCC segment.

The fifth link carries the mass of the soft segment in the simplified augmented model.