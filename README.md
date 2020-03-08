## Navigating Car on Surface Optimally

We seek to use Pointryagin's Maximum Principle to minimize a linear combination of time and gas usage to get a car from point A to point B on a surface.

## Dynamics

The dynamics can be defined as 

\begin{align*}  
  \dot{p} &= vT \\  
  \dot{v} &= u_1 - g T_3 \\  
  \dot{\theta} &= u_2 \\  
\end{align*}

where T is the unit tangent vector (aka directional derivative). A lot was simplified by noting that we only want our car to be moved in the direction it's facing - i.e. gravity won't push it down the hill sideways. This allows us to treat the velocity and acceleration as scalars rather than vectors, making everything a LOT easier.

Further we combined the normal and gravitational acceleration (normally g, and g cos(phi) respectively, where phi is angle of hill) into g sin(phi), which after some tedious trig, is actually just the z component of the unit tangent vector - g*T_3.
