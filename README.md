# WavePropagAnim
Wave propagation animation 
The script solves and animates a two-dimensional wave equation on a rectangular grid using numerical methods for both Dirichlet and Neumann boundary conditions. It begins by defining a Gaussian function as the initial condition and then sets up a system of partial differential equations (PDEs) representing the wave equation, discretized in space and time. The `odeint` function from `scipy.integrate` is used to solve the PDE system over a specified time range. The results are then animated using `matplotlib`, with an option to save the animation as a GIF or individual frames. The animation shows how the wave evolves over time, allowing visualization of the solution under different boundary conditions.

the equation in LaTeX format :
\[
\frac{\partial^2 u}{\partial t^2} = c^2 \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} \right)
\]

Note:
1- Dirichlet Boundary Condition: This specifies the value of the function itself at the boundary. For example, if 
𝑢 (𝑥,𝑦,𝑡) represents the temperature or displacement, the Dirichlet boundary condition sets a fixed value for 
𝑢 at the edges of the domain. In the context of the wave equation, a Dirichlet boundary might mean that the edges of the grid remain at zero displacement, representing a fixed boundary that cannot move (e.g., a string fixed at both ends).

2- Neumann Boundary Condition: This specifies the value of the derivative (usually the normal derivative) of the function at the boundary. For example, it sets a fixed rate of change for 𝑢 at the boundary, which could represent a situation where the flux or slope at the boundary is constant. In the wave equation, a Neumann boundary might mean that the derivative of 𝑢 (such as the slope or velocity) is zero at the edges, allowing the boundary to move freely but without any net change in flux across it (e.g., an insulated or free end of a string).

Enjoy 
