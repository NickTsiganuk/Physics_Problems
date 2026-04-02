## 1. Gravitational Dependence

> **Task:** A simple pendulum has a period of **4 s** on Earth. What would its period be on the Moon, where the gravitational acceleration is about 1/6th of Earth's? What is the required length of a simple pendulum to have a period of exactly **1 s** on Earth?

### Period on the Moon
The formula for the period of a simple pendulum is:
$$T = 2\pi\sqrt{\frac{L}{g}}$$
This shows that the period is inversely proportional to the square root of gravitational acceleration. Setting up a ratio between the period on the Moon and the period on Earth:
$$\frac{T_M}{T_E} = \sqrt{\frac{g_E}{g_M}}$$
Given that gravity on the Moon is 1/6th of Earth's gravity:
$$g_M = \frac{g_E}{6}$$
Substituting this into our ratio:
$$T_M = T_E \sqrt{6}$$
$$T_M = 4 \sqrt{6} \approx 9.80\text{ s}$$

### Length for a 1-second period on Earth
Using the period formula, we can isolate the length:
$$L = \frac{T^2 g}{4\pi^2}$$
Assuming standard Earth gravity is **9.8 m/s²** and substituting **1 s** for the period:
$$L = \frac{1^2 \cdot 9.8}{4\pi^2} \approx 0.248\text{ m}$$

---

## 2. Harmonic Motion

> **Task:** A **10 kg** mass is attached to a spring and oscillates according to the equation $x(t) = 0.2 \cos(10\pi t)$ (in meters). What is the spring constant $k$? What is the total mechanical energy of the system?

### Spring Constant
The general equation for the position of an object in simple harmonic motion is:
$$x(t) = A \cos(\omega t + \phi)$$
By comparing this to the given equation, the angular frequency is:
$$\omega = 10\pi\text{ rad/s}$$
The relationship between angular frequency, mass, and the spring constant is:
$$\omega = \sqrt{\frac{k}{m}}$$
Solving for the spring constant gives:
$$k = m\omega^2$$
$$k = 10 \cdot (10\pi)^2 = 1000\pi^2 \approx 9869.6\text{ N/m}$$

### Total Mechanical Energy
The total energy in a simple harmonic oscillator depends on the spring constant and the amplitude (**0.2 m**):
$$E = \frac{1}{2}kA^2$$
$$E = \frac{1}{2}(1000\pi^2)(0.2)^2 = 20\pi^2 \approx 197.4\text{ J}$$

---

## 3. Conservation of Energy

> **Task:** A pendulum with a length of **1.0 m** is released from an initial angle of **15°**. What is the speed of the pendulum bob at the bottom of its swing?

First, determine the change in height of the pendulum bob from its release point to the bottom of the swing. The height relates to the length and the angle:
$$h = L - L\cos\theta = L(1 - \cos\theta)$$
Using the principle of conservation of energy, the potential energy at the top equals the kinetic energy at the bottom:
$$mgh = \frac{1}{2}mv^2$$
The mass cancels out. Solving for velocity gives:
$$gh = \frac{1}{2}v^2$$
$$2gh = v^2$$
$$v = \sqrt{2gL(1 - \cos\theta)}$$
Substitute the values (**1.0 m** length, **15°**, **9.8 m/s²** for gravity):
$$v = \sqrt{2 \cdot 9.8 \cdot 1.0 \cdot (1 - \cos 15^\circ)}$$
$$v = \sqrt{19.6 \cdot (1 - 0.9659)} \approx \sqrt{0.668} \approx 0.817\text{ m/s}$$

---

## 4. Energy & Momentum

> **Task:** A **0.5 kg** block slides down a frictionless track from a height of **3.0 m**. At the bottom, it collides and sticks to a **1.5 kg** block, which is initially at rest. What is the speed of the combined mass just after the collision?

### Step 1: Velocity before the collision
Use conservation of energy to find the speed of the **0.5 kg** block at the bottom of the track:
$$mgh = \frac{1}{2}mv_1^2$$
$$v_1 = \sqrt{2gh}$$
$$v_1 = \sqrt{2 \cdot 9.8 \cdot 3.0} \approx 7.67\text{ m/s}$$

### Step 2: Velocity after the collision
Because the blocks stick together, this is a perfectly inelastic collision. Apply conservation of momentum:
$$m_1 v_1 = (m_1 + m_2) v_f$$
$$v_f = \frac{m_1 v_1}{m_1 + m_2}$$
$$v_f = \frac{0.5 \cdot 7.67}{0.5 + 1.5} = \frac{3.835}{2.0} \approx 1.92\text{ m/s}$$

---

## 5. Inelastic Collision

> **Task:** A **70 kg** runner moving at **3 m/s** jumps onto a **140 kg** stationary cart. What is the final speed of the cart with the runner? Is kinetic energy conserved in this collision? Explain.

### Final Speed
Apply conservation of momentum where the runner jumps onto the stationary cart:
$$m_r v_r = (m_r + m_c) v_f$$
$$v_f = \frac{m_r v_r}{m_r + m_c}$$
$$v_f = \frac{70 \cdot 3}{70 + 140} = \frac{210}{210} = 1\text{ m/s}$$

### Is kinetic energy conserved?
No. In a perfectly inelastic collision (where objects stick together), kinetic energy is never conserved. The "lost" kinetic energy is dissipated as heat, sound, or internal deformation during the impact.
We can prove this by calculating initial and final kinetic energies:
$$K_i = \frac{1}{2} m_r v_r^2 = \frac{1}{2} \cdot 70 \cdot 3^2 = 315\text{ J}$$
$$K_f = \frac{1}{2} (m_r + m_c) v_f^2 = \frac{1}{2} \cdot 210 \cdot 1^2 = 105\text{ J}$$

---

## 6. Energy Dissipation

> **Task:** A tennis ball is dropped from a height of **2.0 m**. After each bounce, it loses **30%** of its mechanical energy. To what height does it rise after the second bounce?

Losing **30%** of mechanical energy means the ball retains **70%** of its energy after each bounce. Because potential energy is proportional to height, the height retained after each bounce is also **70%** of the previous height.
$$h_1 = 0.7 \cdot h_0$$
After the second bounce:
$$h_2 = 0.7 \cdot h_1 = 0.7^2 \cdot h_0$$
$$h_2 = 0.49 \cdot 2.0 = 0.98\text{ m}$$

---

## 7. Dynamics with Friction

> **Task:** A **5 kg** block is placed on a **10 kg** block. A horizontal force of **45 N** is applied to the **10 kg** block, and the **5 kg** block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is **0.2**. Find the acceleration of the **10 kg** block.

The **5 kg** block is tied to the wall, meaning it remains stationary relative to the ground while the **10 kg** block slides out from underneath it.

1. **Friction between the 5 kg and 10 kg blocks:** The normal force is the weight of the top block.
$$f_1 = \mu_k \cdot m_{\text{top}} \cdot g$$
$$f_1 = 0.2 \cdot 5 \cdot 9.8 = 9.8\text{ N}$$

2. **Friction between the 10 kg block and the floor:** The normal force on the floor is the combined weight of both blocks.
$$f_2 = \mu_k \cdot (m_{\text{top}} + m_{\text{bottom}}) \cdot g$$
$$f_2 = 0.2 \cdot 15 \cdot 9.8 = 29.4\text{ N}$$

3. **Net Force and Acceleration:** The applied force on the **10 kg** block is opposed by both frictional forces.
$$F_{\text{net}} = F_{\text{applied}} - f_1 - f_2$$
$$F_{\text{net}} = 45 - 9.8 - 29.4 = 5.8\text{ N}$$
Using Newton's Second Law for the bottom block:
$$a = \frac{F_{\text{net}}}{m_{\text{bottom}}}$$
$$a = \frac{5.8}{10} = 0.58\text{ m/s}^2$$

---

## 8. Work of a variable force

> **Task:** Given a one-dimensional force: $F(x)=-kx$
> * Write down the equation of motion and solve it.
> * Calculate the work done during the displacement from $0$ to $x_0$.
> * Interpret the result as potential energy.
> * Verify the relationship $F = -\frac{dU}{dx}$.
> * Draw the graph of $F(x)$ and $U(x)$.

### Equation of Motion
Using Newton's Second Law:
$$m\frac{d^2x}{dt^2} = -kx$$
The solution to this differential equation describes simple harmonic motion:
$$x(t) = A\cos\left(\sqrt{\frac{k}{m}}t + \phi\right)$$

### Work Done
Work is the integral of force over displacement:
$$W = \int_{0}^{x_0} F(x) dx$$
$$W = \int_{0}^{x_0} -kx dx = \left[ -\frac{1}{2}kx^2 \right]_{0}^{x_0} = -\frac{1}{2}kx_0^2$$

### Interpretation
The work done by the conservative spring force is negative because the force acts opposite to the displacement. The change in potential energy is defined as the negative of the work done by the conservative force:
$$\Delta U = -W = \frac{1}{2}kx_0^2$$

### Verification
Given the potential energy function:
$$U(x) = \frac{1}{2}kx^2$$
Take the negative derivative with respect to position:
$$-\frac{dU}{dx} = -\frac{d}{dx}\left(\frac{1}{2}kx^2\right) = -kx = F(x)$$

### Graph of F(x) and U(x)
*(To visualize this programmatically, you can plot it using the Python code below. The force $F = -kx$ graphs as a straight line with a negative slope through the origin, while the potential energy $U = 0.5kx^2$ graphs as an upward-opening parabola with its vertex at the origin).*

```python
import numpy as np
import matplotlib.pyplot as plt

x = np.linspace(-5, 5, 100)
k = 2  # arbitrary spring constant

F = -k * x
U = 0.5 * k * x**2

plt.plot(x, F, label="F(x) = -kx")
plt.plot(x, U, label="U(x) = 1/2 kx^2")
plt.xlabel("Displacement (x)")
plt.ylabel("Magnitude")
plt.axhline(0, color='black', linewidth=0.5)
plt.axvline(0, color='black', linewidth=0.5)
plt.legend()
plt.title("Force and Potential Energy of a Spring")
plt.grid(True)
plt.show()
```

---

## 9. Vertical throw with drag

> **Task:** We have the equation of motion: $m\frac{dv}{dt} = -mg - kv$ with initial conditions $v(0)=v_0$, $x(0)=10$.
> * Solve the equation by analytical methods.
> * Determine the maximum height.
> * Compare with the case without drag.
> * Perform a numerical simulation using HTML or Python.

### Analytical Solution
The equation of motion is:
$$m\frac{dv}{dt} = -mg - kv$$
Rearrange to separate variables:
$$\frac{dv}{g + \frac{k}{m}v} = -dt$$
Integrate both sides from initial velocity to arbitrary velocity:
$$\int_{v_0}^{v} \frac{dv}{g + \frac{k}{m}v} = \int_{0}^{t} -dt$$
$$\frac{m}{k} \ln\left( \frac{g + \frac{k}{m}v}{g + \frac{k}{m}v_0} \right) = -t$$
Solve for velocity:
$$v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t} - \frac{mg}{k}$$

### Maximum Height
Max height occurs when velocity reaches zero:
$$0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t_{\text{max}}} - \frac{mg}{k}$$
$$t_{\text{max}} = \frac{m}{k} \ln\left( 1 + \frac{kv_0}{mg} \right)$$
Integrate the velocity function to find position, then substitute $t_{\text{max}}$ to get the exact maximum height.

### Comparison
Without drag, the maximum height is derived simply from energy conservation:
$$H_{\text{no\_drag}} = 10 + \frac{v_0^2}{2g}$$
With aerodynamic drag pulling down during the ascent, kinetic energy is depleted faster, resulting in a lower maximum height.

### Numerical Simulation (Python)
```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.integrate import solve_ivp

# Parameters
m = 1.0; g = 9.8; k = 0.5; v0 = 20.0; y0 = 10.0

def equations(t, y):
    pos, vel = y
    dydt = vel
    dvdt = -g - (k/m)*vel
    return [dydt, dvdt]

# Stop condition: when velocity is 0 (max height) or reaches ground (y=0)
def event_ground(t, y): return y[0]
event_ground.terminal = True

sol = solve_ivp(equations, [0, 5], [y0, v0], events=event_ground, dense_output=True)

t = np.linspace(0, sol.t[-1], 100)
y = sol.sol(t)[0]

plt.plot(t, y)
plt.title("Vertical Throw with Drag")
plt.xlabel("Time (s)")
plt.ylabel("Height (m)")
plt.grid(True)
plt.show()
```

---

## 10. Force field and power

> **Task:** In a certain force field, the equations of motion of a particle with mass $m=0.5$ kg are as follows: $x = 5t^2 - t, \quad y = 2t^3, \quad z = -3t + 2$. Find the time dependence of: the particle's velocity, the particle's momentum, the particle's acceleration, the force acting on the particle, and the power transferred by the field to the particle.

Given the position vector:
$$\vec{r}(t) = (5t^2 - t)\hat{i} + 2t^3\hat{j} + (-3t + 2)\hat{k}$$

### Velocity
Take the first time derivative of position:
$$\vec{v}(t) = \frac{d\vec{r}}{dt} = (10t - 1)\hat{i} + 6t^2\hat{j} - 3\hat{k}$$

### Momentum
Multiply velocity by mass (**0.5 kg**):
$$\vec{p}(t) = m\vec{v}(t) = (5t - 0.5)\hat{i} + 3t^2\hat{j} - 1.5\hat{k}$$

### Acceleration
Take the time derivative of velocity:
$$\vec{a}(t) = \frac{d\vec{v}}{dt} = 10\hat{i} + 12t\hat{j} + 0\hat{k}$$

### Force
Multiply acceleration by mass:
$$\vec{F}(t) = m\vec{a}(t) = 5\hat{i} + 6t\hat{j} + 0\hat{k}$$

### Power
Power is the dot product of force and velocity:
$$P(t) = \vec{F}(t) \cdot \vec{v}(t)$$
$$P(t) = 5(10t - 1) + 6t(6t^2) + 0(-3)$$
$$P(t) = 50t - 5 + 36t^3\text{ W}$$

---

## 11. Dynamics with a time-dependent force

> **Task:** A particle of mass $m=3$ kg moves in a force field $F$ dependent on time in the following way: $F = (15t, 3t-12, -6t^2)$ N. Assuming initial conditions $r_0=(5,2,-3)$ m, $v_0=(2,0,1)$ m/s, find the dependence of the particle's position and velocity on time.

Given mass (**3 kg**) and force:
$$\vec{F}(t) = (15t, 3t - 12, -6t^2)\text{ N}$$
$$\vec{a}(t) = \frac{\vec{F}}{m} = (5t, t - 4, -2t^2)\text{ m/s}^2$$

### Velocity
Integrate acceleration and apply the initial velocity conditions (2, 0, 1):
$$v_x(t) = \int 5t dt = \frac{5}{2}t^2 + 2$$
$$v_y(t) = \int (t - 4) dt = \frac{1}{2}t^2 - 4t + 0$$
$$v_z(t) = \int -2t^2 dt = -\frac{2}{3}t^3 + 1$$

### Position
Integrate velocity and apply initial position conditions (5, 2, -3):
$$x(t) = \int \left( \frac{5}{2}t^2 + 2 \right) dt = \frac{5}{6}t^3 + 2t + 5$$
$$y(t) = \int \left( \frac{1}{2}t^2 - 4t \right) dt = \frac{1}{6}t^3 - 2t^2 + 2$$
$$z(t) = \int \left( -\frac{2}{3}t^3 + 1 \right) dt = -\frac{1}{6}t^4 + t - 3$$

---

## 12. Work and energy with a constant force

> **Task:** A constant force acts on a body of mass $m = 2$ kg: $\vec F = [6, 2]$ N. The body starts with an initial velocity $\vec v(0) = (1, -1)$ m/s from the point $\vec r(0)=(0,0)$ m.
> * Determine $\vec a(t)$.
> * Determine $\vec v(t)$.
> * Determine $\vec r(t)$.
> * Draw the trajectory of the motion.
> * Calculate the work done by the force at time $t=3$ s.
> * Check the consistency with the work-energy theorem.

### Acceleration
$$\vec{a} = \frac{\vec{F}}{m} = \left(\frac{6}{2}, \frac{2}{2}\right) = (3, 1)\text{ m/s}^2$$

### Velocity
$$\vec{v}(t) = \vec{a}t + \vec{v}(0) = (3t + 1, t - 1)\text{ m/s}$$

### Position
$$\vec{r}(t) = \frac{1}{2}\vec{a}t^2 + \vec{v}(0)t + \vec{r}(0) = (1.5t^2 + t, 0.5t^2 - t)\text{ m}$$

### Trajectory Graph
```python
import numpy as np
import matplotlib.pyplot as plt

t = np.linspace(0, 4, 50)
x = 1.5 * t**2 + t
y = 0.5 * t**2 - t

plt.plot(x, y)
plt.title("Trajectory of the Body")
plt.xlabel("x Position (m)")
plt.ylabel("y Position (m)")
plt.grid(True)
plt.show()
```

### Work Done at t = 3 s
Calculate the position at **3 s**:
$$\vec{r}(3) = (1.5(3)^2 + 3, 0.5(3)^2 - 3) = (16.5, 1.5)\text{ m}$$
Because the force is constant, work is the dot product of force and displacement:
$$W = \vec{F} \cdot \vec{r}(3)$$
$$W = (6)(16.5) + (2)(1.5) = 99 + 3 = 102\text{ J}$$

### Consistency with Work-Energy Theorem
The theorem states the work done is equal to the change in kinetic energy. Let's find the initial and final kinetic energies:
$$K_i = \frac{1}{2}m|\vec{v}(0)|^2 = \frac{1}{2}(2)(1^2 + (-1)^2) = 2\text{ J}$$
Calculate velocity at **3 s**:
$$\vec{v}(3) = (3(3) + 1, 3 - 1) = (10, 2)\text{ m/s}$$
$$K_f = \frac{1}{2}m|\vec{v}(3)|^2 = \frac{1}{2}(2)(10^2 + 2^2) = 104\text{ J}$$
$$\Delta K = K_f - K_i = 104 - 2 = 102\text{ J}$$
The calculated work completely matches the change in kinetic energy, satisfying the theorem.