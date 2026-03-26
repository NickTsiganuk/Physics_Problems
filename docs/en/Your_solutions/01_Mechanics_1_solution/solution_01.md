
## 1. Projectile Motion

> **Task:** A projectile is fired from the ground with an initial velocity of 100 m/s at an angle of 37° above the horizontal. Assume no air resistance. 
> * Derive the differential equations of motion in the horizontal and vertical directions.
> * Determine the time of flight.
> * Determine the maximum height.
> * Determine the range.

**Solution:**
We are given an initial velocity $v_0$ of 100 m/s and an angle $\theta$ of 37°. We will use the acceleration due to gravity $g \approx 9.8\text{ m/s}^2$. For simplicity, we will use the standard geometric approximations $\sin(37^\circ)\approx 0.6$ and $\cos(37^\circ)\approx 0.8$.

* **Differential equations of motion:**
  Assuming the origin is at the launch point, gravity acts purely in the negative vertical direction.
  * Horizontal: $$\frac{d^2x}{dt^2}=0$$
  * Vertical: $$\frac{d^2y}{dt^2}=-g$$
* **Time of flight ($T$):**
  The vertical position equation is $y(t)=v_0\sin(\theta)t-\frac{1}{2}gt^2$. The projectile lands when $y(t)=0$.
  $$0=t\left(v_0\sin(\theta)-\frac{1}{2}gt\right)$$
  $$T=\frac{2v_0\sin(\theta)}{g}=\frac{2(100)(0.6)}{9.8}\approx 12.24\text{ s}$$
* **Maximum height ($H$):**
  Maximum height occurs when the vertical velocity $v_y=v_0\sin(\theta)-gt=0$, which is at half the flight time ($t=T/2$). Substituting this back into the $y(t)$ equation gives:
  $$H=\frac{(v_0\sin\theta)^2}{2g}=\frac{(100\times 0.6)^2}{2\times 9.8}=\frac{3600}{19.6}\approx 183.67\text{ m}$$
* **Range ($R$):**
  The horizontal position equation is $x(t)=v_0\cos(\theta)t$. Substitute the total time of flight $T$:
  $$R=v_0\cos(\theta)\times T=100(0.8)(12.24)\approx 979.2\text{ m}$$

---

## 2. Range Optimization
For projectile motion, show analytically that the maximum range $R(\theta)=\frac{v_0^2 \sin(2\theta)}{g}
$ for a given initial velocity is achieved at a launch angle of $45^\circ$.

### The Goal
We want to prove that a projectile will travel the furthest horizontal distance (the "range") if you launch it at exactly a 45° angle, assuming you always launch it with the exact same initial speed. 

We are given the formula for the range:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

In this formula:
* $v_0$ is the initial launch velocity (a constant).
* $g$ is the acceleration due to gravity (a constant).
* $\theta$ is the launch angle (our variable). 

Since $v_0$ and $g$ are constant, the only thing that changes the range $R$ is the angle $\theta$.

---

### Step 1: Take the Derivative
In calculus, the derivative tells us the "slope" of our function. When a curve reaches its highest peak (the maximum range), it flattens out for a split second, meaning its slope is exactly zero. 

To find that peak, we first need to take the derivative of the range $R$ with respect to the angle $\theta$:
$$\frac{dR}{d\theta} = \frac{d}{d\theta} \left( \frac{v_0^2 \sin(2\theta)}{g} \right)$$

Because $\frac{v_0^2}{g}$ is just a constant multiplier, we can pull it out of the derivative. We only need to differentiate $\sin(2\theta)$. Using the chain rule, the derivative of $\sin(2\theta)$ is $2\cos(2\theta)$. 

So, our derivative becomes:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta) = \frac{2v_0^2\cos(2\theta)}{g}$$

### Step 2: Set the Derivative to Zero
Now that we have an equation for the slope, we want to find out where the slope is perfectly flat. We do this by setting our derivative equal to 0:
$$\frac{2v_0^2\cos(2\theta)}{g} = 0$$

### Step 3: Solve for the Angle ($\theta$)
Now we just need to solve for $\theta$. 

Look at the fraction: $\frac{2v_0^2}{g}$. Because we assume the projectile is actually moving ($v_0$ is not zero) and gravity exists ($g$ is not zero), this fraction cannot equal zero. 

For the whole equation to equal zero, the trigonometric part must be the thing that equals zero:
$$\cos(2\theta) = 0$$

Now we ask ourselves: at what angle does the cosine function equal zero? Cosine is zero at 90°. Therefore, the inside of our cosine function must equal 90°:
$$2\theta = 90^\circ$$

Divide by 2:
$$\theta = 45^\circ$$

## 3. Path Intersection

> **Task:** Alice is moving along a path described by $A(t)=(2+t, 8-3t)$ and Bob is moving along a path $B(t)=(2t-1, 2t+2)$. Determine if their paths intersect. If yes, determine when and where they will collide. If not, determine the minimum distance between them and when it occurs.

**Solution:**
**1. Do the paths intersect in space?**
Let's eliminate $t$ to find the spatial equations $y(x)$.
* **Alice:** $x=2+t \Rightarrow t=x-2$. Substitute into $y$: $y=8-3(x-2)=14-3x$.
* **Bob:** $x=2t-1 \Rightarrow t=\frac{x+1}{2}$. Substitute into $y$: $y=2\left(\frac{x+1}{2}\right)+2=x+3$.

Set $y_A=y_B$ to find the intersection point:
$$14-3x=x+3 \Rightarrow 4x=11 \Rightarrow x=2.75$$
$$y=2.75+3=5.75$$
**Yes, the paths intersect at the coordinates (2.75, 5.75).**

**2. Do they collide?**
A collision only happens if they reach that point at the *same time*. Let's set their $x(t)$ equations equal:
$$2+t=2t-1 \Rightarrow t=3\text{ s}$$
At $t=3$ s, Alice is at $y_A=8-3(3)=-1$. Bob is at $y_B=2(3)+2=8$. They are not at the same $y$-coordinate at that time. **Therefore, they do not collide.**

**3. Minimum distance:**
The distance squared between them at any time $t$ is $D^2=(x_B-x_A)^2+(y_B-y_A)^2$.
$$D^2=((2t-1)-(2+t))^2+((2t+2)-(8-3t))^2$$
$$D^2=(t-3)^2+(5t-6)^2=t^2-6t+9+25t^2-60t+36=26t^2-66t+45$$
To minimize $D^2$, find where its derivative is zero:
$$\frac{d(D^2)}{dt}=52t-66=0 \Rightarrow t=\frac{66}{52}\approx 1.27\text{ s}$$
Substitute $t\approx 1.27$ back into the distance formula:
$$D_{min}=\sqrt{26(1.27)^2-66(1.27)+45}\approx 1.76\text{ units}$$

---

## 4. Vector Calculus

> **Task:** The position of an object is given by $\vec{r}(t)=(3t^2)\hat{i}+(5t-8t^2)\hat{j}$. Find the object's velocity and acceleration vectors as a function of time.

**Solution:**
We start with the position vector: $\vec{r}(t)=(3t^2)\hat{i}+(5t-8t^2)\hat{j}$.

* **Velocity:** Take the first derivative of position with respect to time.
  $$\vec{v}(t)=\frac{d\vec{r}}{dt}=(6t)\hat{i}+(5-16t)\hat{j}$$
* **Acceleration:** Take the second derivative (or the derivative of velocity).
  $$\vec{a}(t)=\frac{d\vec{v}}{dt}=6\hat{i}-16\hat{j}$$

---

## 5. Relative Velocity

> **Task:** A river flows east at 2 m/s. A boat that can travel at 5 m/s in still water wants to go directly north across the river. In what direction (angle) should it head? How long will it take to cross the river if it's 200 meters wide?

**Solution:**
* **Heading Direction:**
  The boat wants its resultant velocity vector to point straight north. The river is pushing it east at 2 m/s. Therefore, the boat must head slightly west of north so its westward velocity component perfectly cancels out the river's eastward current. Let $\theta$ be the angle west of north.
  $$v_{boat}\sin(\theta)=v_{river} \Rightarrow 5\sin(\theta)=2 \Rightarrow \sin(\theta)=0.4$$
  $$\theta=\arcsin(0.4)\approx 23.6^\circ\text{ west of north}$$
* **Crossing Time:**
  The boat's effective speed moving straight north is the vertical component of its velocity:
  $$v_{north}=5\cos(23.6^\circ)=5\sqrt{1-0.4^2}=5\sqrt{0.84}\approx 4.58\text{ m/s}$$
  Time to cross a 200-meter river:
  $$t=\frac{d}{v_{north}}=\frac{200}{4.58}\approx 43.6\text{ s}$$

---

## 6. Variable Velocity

> **Task:** An object's velocity is given by $v(t)=t^2+2t-5$. If the object was at $x=4$ at $t=0$, what is its position and acceleration at time $t=3$?

**Solution:**
* **Position:** Integrate velocity to find $x(t)$.
  $$x(t)=\int(t^2+2t-5)dt=\frac{t^3}{3}+t^2-5t+C$$
  Using the initial condition $x(0)=4$, we find $C=4$. So, $x(t)=\frac{t^3}{3}+t^2-5t+4$.
  At $t=3$:
  $$x(3)=\frac{3^3}{3}+3^2-5(3)+4=9+9-15+4=7$$
* **Acceleration:** Differentiate velocity to find $a(t)$.
  $$a(t)=\frac{dv}{dt}=2t+2$$
  At $t=3$:
  $$a(3)=2(3)+2=8$$

---

## 7. Elimination of Time and Interpretation of Acceleration

> **Task:** The path equation is given in parametric form: 
> $$x(t)=2t^2, \qquad y(t)=3t^3$$ 
> * Eliminate the parameter $t$. 
> * Draw the trajectory. 
> * Calculate $\vec{v}(t)$, $|\vec{v}(t)|$, $\vec{a}(t)$ and $|\vec{a}(t)|$. 
> * Is the acceleration constant?

**Solution:**
* **Eliminate $t$:**
  From the $x$ equation, assuming $t \geq 0$, $t=\sqrt{x/2}$. Substitute this into $y(t)$:
  $$y(x)=3\left(\sqrt{\frac{x}{2}}\right)^3=3\sqrt{\frac{x^3}{8}}$$
  Squaring both sides gives the algebraic equation: $y^2=\frac{9}{8}x^3$.
* **Trajectory Shape:**
  This curve is known as a semicubical parabola. It has a cusp at the origin (0,0) and opens outward primarily in the positive $x$ direction. 
* **Vectors and Magnitudes:**
  * Velocity: $\vec{v}(t)=\frac{d\vec{r}}{dt}=(4t, 9t^2)$
  * Speed: $|\vec{v}(t)|=\sqrt{(4t)^2+(9t^2)^2}=\sqrt{16t^2+81t^4}=t\sqrt{16+81t^2}$
  * Acceleration: $\vec{a}(t)=\frac{d\vec{v}}{dt}=(4, 18t)$
  * Accel. Magnitude: $|\vec{a}(t)|=\sqrt{4^2+(18t)^2}=\sqrt{16+324t^2}$
* **Is acceleration constant?**
  **No.** While the $x$-component is constant (4), the $y$-component ($18t$) changes with time. Since the vector changes, the overall acceleration is not constant.

---

## 8. Circular Motion

> **Task:** Calculate the centripetal acceleration of a person standing on the Earth's equator. The Earth's radius is approximately 6378 km.

**Solution:**
* Earth's radius $R = 6378$ km = 6,378,000 m.
* Time for one rotation $T \approx 24$ hours = 86,400 s.
* Angular velocity $\omega=\frac{2\pi}{T}=\frac{2\pi}{86400}\approx 7.27\times 10^{-5}\text{ rad/s}$.
* Centripetal acceleration $a_c=\omega^2R$:
  $$a_c=(7.27\times 10^{-5})^2\times 6,378,000\approx 0.0337\text{ m/s}^2$$

---

## 9. Momentum Comparison

> **Task:** Which has greater momentum: a 2-gram fly flying at 10 m/s or a 60-gram tennis ball moving at 1 m/s?

**Solution:**
Momentum is calculated as $p=m\times v$.
* **Fly:** $m = 2$ g = 0.002 kg. $v = 10$ m/s.
  $$p_{fly}=0.002\times 10=0.02\text{ kg}\cdot\text{m/s}$$
* **Tennis Ball:** $m = 60$ g = 0.06 kg. $v = 1$ m/s.
  $$p_{ball}=0.06\times 1=0.06\text{ kg}\cdot\text{m/s}$$

**The tennis ball has greater momentum.**

---

## 10. Kinematics

> **Task:** Point M moves according to the equation: 
> $$\vec{r}(t)=(a\cos(\omega t), b\sin(\omega t), bt)$$ 
> where $a, b, \omega$ are positive constants. 
> a) Find the equation of the point's trajectory, 
> b) Compute the path length of the point from time $t=0$ to $t=t_0$, 
> c) Draw the trajectory of this point using Python or interactive HTML. Discuss special cases.

**Solution:**
**a) Equation of the trajectory:**
Isolate $\cos(\omega t)$ and $\sin(\omega t)$ to eliminate time from the $x$ and $y$ planes:
$$x=a\cos(\omega t) \Rightarrow \frac{x}{a}=\cos(\omega t)$$
$$y=b\sin(\omega t) \Rightarrow \frac{y}{b}=\sin(\omega t)$$
Squaring and adding them yields the identity $\sin^2(\theta)+\cos^2(\theta)=1$:
$$\frac{x^2}{a^2}+\frac{y^2}{b^2}=1$$
This shows the trajectory is bounded within an elliptical cylinder in 3D space. The particle spirals upward along the $z$-axis ($z=bt$), making the trajectory an **elliptical helix**.

**b) Path length from $t=0$ to $t=t_0$:**
First, find the velocity vector components:
$v_x=-a\omega\sin(\omega t)$, $v_y=b\omega\cos(\omega t)$, $v_z=b$.
The speed is:
$$|\vec{v}|=\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)+b^2}$$
The path length $S$ is the integral of speed:
$$S=\int_0^{t_0}\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)+b^2}dt$$
*Note: Because $a$ and $b$ are not necessarily equal, this results in an incomplete elliptic integral of the second kind, which generally does not have a simple closed-form solution in terms of elementary functions unless $a=b$.*

**c) Python Code for Trajectory & Discussion:**
Here is a Python script using `matplotlib` to plot the trajectory.

```python
import numpy as np
import matplotlib.pyplot as plt

# Constants (you can change these to explore special cases)
a = 5.0
b = 3.0
omega = 2.0
t_0 = 10.0

# Generate time values
t = np.linspace(0, t_0, 1000)

# Parametric equations
x = a * np.cos(omega * t)
y = b * np.sin(omega * t)
z = b * t

# Plotting
fig = plt.figure(figsize=(8, 8))
ax = fig.add_subplot(111, projection='3d')
ax.plot(x, y, z, label='Elliptical Helix', color='b')

ax.set_xlabel('X axis')
ax.set_ylabel('Y axis')
ax.set_zlabel('Z axis')
ax.set_title('Trajectory of Point M')
ax.legend()
plt.show()
```

**Discussion of special cases:**
* **$a=b$:** The equation becomes $x^2+y^2=a^2$. The base is a perfect circle, and the curve is a standard circular helix (like a typical spring). The path length integral also simplifies nicely into a linear relation because the speed becomes constant.
* **$a=0$ or $b=0$:** If $b=0$, the particle simply oscillates back and forth along the $x$-axis from $x=a$ to $x=-a$ because $y=0$ and $z=0$. If $a=0$, it oscillates on the $y$-axis while simultaneously moving steadily up the $z$-axis (resulting in a 2D sine wave traced on the $yz$-plane).
* **$\omega=0$:** The particle remains at $x=a, y=0$ while moving steadily up the $z$-axis at speed $b$. The path is a straight vertical line.

---