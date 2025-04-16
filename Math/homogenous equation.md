### Solving First-Order Homogeneous ODEs

For ODEs of the form $dydx=f(yx)\frac{dy}{dx} = f\left(\frac{y}{x}\right)dxdy​=f(xy​)$, use the **substitution** v=yxv = \frac{y}{x}v=xy​, where y=vxy = vxy=vx and dydx=v+xdvdx\frac{dy}{dx} = v + x\frac{dv}{dx}dxdy​=v+xdxdv​. Substituting into the ODE yields:

v+xdvdx=f(v)v + x \frac{dv}{dx} = f(v)v+xdxdv​=f(v)

This reduces the problem to a separable ODE:

dvf(v)−v=dxx\frac{dv}{f(v) - v} = \frac{dx}{x}f(v)−vdv​=xdx​

Solve for vvv, then substitute back y=vxy = vxy=vx.