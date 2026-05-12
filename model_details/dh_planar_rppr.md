# Planar RPPR DH Parametrization

This file provides the Denavit--Hartenberg (DH) parametrization of the planar RPPR augmented rigid-body chain used for one PCC segment.

## Augmented coordinates

For a planar PCC segment, the augmented coordinates are

```math
\xi_i = [h_1,\ d_1,\ d_2,\ h_2]^\top \in \mathbb{R}^4 .
```

The curvature-to-ARBM mapping used in the paper is

```math
m_i(q_i)=
\begin{bmatrix}
\tfrac{q_i}{2}, &
L_i\tfrac{\sin(q_i/2)}{q_i}, &
L_i\tfrac{\sin(q_i/2)}{q_i}, &
\tfrac{q_i}{2}
\end{bmatrix}^\top.
```

# DH table

$$
\begin{array}{|c|c|c|c|c|c|}
\text{Link} & \theta & d & a & \alpha & \mu \\
\hline
1 & q_i/2 & 0 & 0 & \pi/2 & 0 \\
2 & 0 & L_i\frac{\sin(q_i/2)}{q_i} & 0 & 0 & \mu_i \\
3 & 0 & L_i\frac{\sin(q_i/2)}{q_i} & 0 & -\pi/2 & 0 \\
4 & q_i/2 & 0 & 0 & 0 & 0
\end{array}
$$

## Description

The RPPR chain is used as an augmented rigid-body representation of a planar constant-curvature segment. The geometric constraint maps the scalar curvature coordinate q_i into the four augmented coordinates of the equivalent rigid chain.

Only the second link carries the mass of the soft segment in the simplified model.