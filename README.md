# WavePropagAnim
Wave propagation animation 
The script solves and animates a two-dimensional wave equation on a rectangular grid using numerical methods for both Dirichlet and Neumann boundary conditions. It begins by defining a Gaussian function as the initial condition and then sets up a system of partial differential equations (PDEs) representing the wave equation, discretized in space and time. The `odeint` function from `scipy.integrate` is used to solve the PDE system over a specified time range. The results are then animated using `matplotlib`, with an option to save the animation as a GIF or individual frames. The animation shows how the wave evolves over time, allowing visualization of the solution under different boundary conditions.

the equation in LaTeX format :
\[
\frac{\partial^2 u}{\partial t^2} = c^2 \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} \right)
\]

Enjoy 
