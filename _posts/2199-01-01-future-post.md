---
title: 'Quantum Tunneling'
date: 2021-05-28
permalink: /posts/2012/08/quantumtunneling/
tags:

---
**Quantum Mechanics and Tunneling**

> The behaviour of most objects that we deal with in our day-to-day life
> can be explained by classical mechanics. Classical physics is causal,
> which means that outcomes are completely predictable given full
> knowledge of the system's past. But what about at the smallest levels
> of the universe? The behaviour of particles is not similarly
> predictable. To study particles, quantum mechanics is what helps us
> understand the behaviour of matter at the subatomic level.
>
> One of many interesting quantum phenomena is quantum tunneling.
> Quantum tunneling describes a particle penetrating through a potential
> barrier. A potential barrier is “a region in which the potential is
> significantly higher than at points on either side of it” and higher
> than the energy of the particle \[1\]. This behaviour is impossible
> for a particle from the perspective of classical physics, as the
> particle simply doesn’t have the energy to do so.
>
> Quantum mechanics describes particles as being wavelike, also known as
> the wave nature of particles. Quantum physics is also probabilistic.
> Predictions of outcomes take the form of probabilities. In the last
> section of this paper we will find the probability that a particle
> penetrates through a potential barrier, i.e. solve the barrier
> tunneling problem. To do this however, we need to first establish the
> relevant mathematical concepts (specifically the method for solving
> second-order differential equations) and classical wave concepts. We
> will then derive Schrödinger’s equation, which is the first step into
> looking at the quantum ideas.
>
> **1. Solving second-order differential equations with constant
> coefficients**
>
> Solving wave equations often involves solving second order
> differential equations. The most common form that will be relevant
> throughout the following sections is
>
> $\frac{d^{2}x}{dt^{2}} - A^{2}x\  = 0.$ (1)
>
> Rearranging, we notice that the second derivative of $x$ is equal to
> the square of the constant *A* multiplied by $x$. This relationship is
> found in exponential functions of $x$. Therefore we can make an
> assumption that $x = e^{\lambda t}$. Substituting this into equation
> (1) we obtain
>
> ${\lambda^{2}e}^{\lambda t} - A^{2}e^{\lambda t}\  = 0.$ (2)
>
> Cancelling the exponential component and finding $\lambda$ in terms of
> $A$ we find
>
> $\lambda = {\pm A}^{}$ (3)
>
> and by substituting back into our assumed form for $x(t)$, we find the
> two solutions
>
> $x = {C_{1}e}^{\text{At}}$ and $x = {C_{2}e}^{- At}.$ (4)
>
> Now there appear to be two solutions - this suggests that we would
> need to take one of the two, or both (as independent solutions).
> However, we can use a useful property of second order linear
> differential equations to obtain one solution depending on two
> parameters. This property is called linearity and it says that for
> linear differential equations, the sum of its solutions will generate
> another solution \[2\]. This property is very relevant when finding
> solutions to wave equations as adding the two solutions allows us to
> generate one solution that incorporates the effect of both of the
> independent motions occurring in a specific system.
>
> For example, in a simple harmonic oscillator, the solutions come in
> the forms $\sin(t)$ and $\cos(t)$. The $\sin(t)$ solution starts with
> some velocity but no displacement, which could occur when you push a
> mass from rest at the equilibrium. On the other hand the cos$(t)$
> solution begins at a position greater than zero, but no velocity,
> which corresponds to pulling the mass away from equilibrium. There are
> two types of motion here. We could combine these by pulling the mass
> away from equilibrium to the same position and then pushing it away
> with some velocity. Linearity says that you would just add the two
> trigonometric solutions to get a solution representing the motion for
> all values of time t.
>
> We can verify that the sum of the solutions is also a solution using
> the general form of a second order linear differential equation
>
> $A\frac{d^{2}x}{dt^{2}} + B\frac{\text{dx}}{\text{dt}} + Cx\  = \ 0,$
> where A, B and C are constant coefficients. (5)
>
> We can consider $x_{1}(t)\ $and $x_{2}(t)$to be the solutions of eq
> (1). Writing the equations in terms of these solutions gives us
>
> $A\frac{d^{2}x_{1}}{dt^{2}} + B\frac{dx_{1}}{\text{dt}} + Cx_{1}\  = \ 0$
> and
> $A\frac{d^{2}x_{2}}{dt^{2}} + B\frac{dx_{2}}{\text{dt}} + Cx_{2}\  = \ 0$.
> (6)
>
> Since these are both equal to zero, we can add the equations, giving
>
> $A\frac{d^{2}{(x}_{1} + x_{2})}{dt^{2}} + B\frac{d{(x}_{1} + x_{2})}{\text{dt}} + C{(x}_{1} + x_{2})\  = \ 0.$
> (7)
>
> Hence ${(x}_{1} + x_{2})(t)$ is also a solution.
>
> Going back to the solutions in equation (4) we can use linearity to
> get the solution
>
> $x = {C_{1}e}^{\text{At}}$$+ {C_{2}e}^{- At}.$
>
> When the second-order differential equation involves a negative
> function of $x,$ the solution will differ slightly. For example,
> consider the equation
>
> $\frac{d^{2}x}{dt^{2}} = A^{2}x$. (8)
>
> Now if we were to substitute $x = e^{\lambda t}$ there is an imaginary
> component introduced because when we solve for $\lambda$ we get
> $\lambda = \pm iA.$ This makes mathematical sense since the
> relationship in equation (4) can only be true when the power of $e$
> contains $i$ (in order for the negative sign to exist).
>
> Hence the two solutions are complex exponentials; $x = Ce^{\pm iAt}$.
> Using linearity we can write the general solution
>
> $x = C_{1}e^{\text{iAt}}$$+ C_{2}e^{- iAt}.$ (9)
>
> For this second case, we could also use a sine or cosine function, as
> the negative of these two types of functions is also proportional to
> the second derivative. Further, we can derive the trigonometric form
> using the complex exponential already found.
>
> We can look at the solution as the summation of two complex numbers,
> since complex exponentials represent complex numbers ( E.g
> ${Be^{i\theta}}^{}$is a complex number with magnitude $B$ and argument
> $\theta$). With this, (9) can be expanded into the polar form of the
> complex numbers to give

$C_{1}\cos(At) + \text{iC}_{1}\sin(At) + C_{2}\cos(At) - \text{iC}_{2}\sin(At)$.
(10)

This simplifies to

${(C}_{1} + C_{2})(\cos(At)) + {i(C}_{1} - C_{2})(\sin(At))$ (11)

> We will find this understanding very useful as second-order
> differential equations will come up continuously throughout the rest
> of the paper.

**2. Concepts from Classical Physics **

> **2.1. Oscillators and waves**
>
> In 1801, Thomas Young’s ‘double slit’ experiment showed us that unlike
> the classical expectation that the particles would end up at one of
> two locations on a detector, the particles sent through a double slit
> actually behaved as waves do. On the detector, the particles formed an
> interference pattern in the way that two coherent waves would. So
> quantum physics describes that “particles have wavelike properties”
> \[2\] and the wave-like behaviour of the particles is determined by a
> wave equation, namely Schrödinger’s equation. Given this, it is
> important to understand classic properties of waves in order to
> explain quantum tunneling of particles. First, we will look at simple
> harmonic motion (SHM), specifically solving for the position $x(t)$ in
> an oscillating mass on a spring (as this also provides the necessary
> prior understanding for looking at the behaviour of waves and solving
> the wave equation).
>
> **2.1.1 SHM and oscillations**
>
> *Solving for* $x(t)$
>
> An object undergoing simple harmonic motion has a restoring force that
> is directly proportional to the object’s displacement acting towards
> the equilibrium of the system. In this section we will look at a mass
> on a spring. Determining the position $x(t)$ can be done by writing
> Newton’s second law of motion in terms of $x$, with the aid of Hooke’s
> law force $F(x)\  = \  - kx$, where $k$ is the spring constant.
>
> Let’s look at Newton’s second law of motion, $F = ma.$
>
> We can substitute the force given in Hooke’s law, giving
>
> $- kx = ma.$ (1)
>
> Now we have two variables, $x$ and $a$ (acceleration). In order to
> solve for $x,$ acceleration should also be written in terms of $x$.
> Acceleration is the second derivative of the position, therefore
> equation (1) becomes
>
> $- kx = m\frac{d{}^{2}x}{dt^{2}}.$ (2)
>
> This now resembles the second-order differential equations we looked
> at in section one so we can apply the same method to solve it.
> Plugging in $x(t) = e^{\beta t}$ we get
>
> $- ke^{\beta t} = m\beta^{2}e^{\beta t}$. (3)
>
> Cancelling the common term $e^{\beta t}$ shows us that
> $\beta^{2} = \frac{\  - k\ }{m}$.
>
> We can now introduce the parameter of angular velocity of the SHM
> system, $\omega.$ It satisfies $\ \omega =$.
>
> Since $\beta^{2} = \frac{- k}{m}\ $ and $\omega =$ we see that
> $\beta = \pm i\omega.$
>
> Therefore the solutions are
>
> $x(t) = Ce^{\pm i\omega t}$, (4)

which (using linearity) can be written as one solution,

$x(t) = C_{1}e^{i\omega t} + C_{2}e^{- i\omega t}.$ (5)

The coefficients $C_{1}$and $C_{2}$ can take any value in order to
satisfy equation (2), complex or real.

> However, we know that $x(t)$ is equal to its own complex conjugate so
> it can be assumed that the two terms are complex conjugates of each
> other. For the complex numbers $C_{1}$and $C_{2}$, we can use the
> exponential form of complex numbers which will make it easier to
> simplify later. Moreover, two parameters of the SHM system (phase,
> $\varphi$ and amplitude, $A$) are now introduced into the solution
> since the exponential form is the product of the magnitude (which can
> be called $A$) and the phase, $e^{i\varphi}$ of the complex number.
> The complex conjugate has equal magnitude and equal but negative
> power.
>
> Hence, equation (5) now expands to
>
> $x(t) = C_{0}e^{i\varphi}e^{i\omega t} + C_{0}e^{- i\varphi}e^{- i\omega t}.$
> (6)
>
> Now expanding equation (6) using polar form as we did in equation (10)
> of section one and then simplifying by collecting like terms, we get
>
> $x(t) = {2C}_{0}\cos(\omega t + \phi).$ (7)
>
> This method is important as it shows how to take the real part of the
> complex solution in order to get a solution that is consistent with
> the physical context of the mass-spring system. Looking back at (2),
> where $x$ is proportional to its second derivative, we can see that
> the solution in (7) is consistent, as the cosine function also
> possesses this relationship with its second derivative.
>
> **2.1.2 Transverse and standing waves**
>
> Transverse waves on a string are governed by the wave equation, which
> we will derive in this section. We will also look at reflection and
> transmission of waves and examine wave behaviour when reaching
> different types of boundaries.
>
> As mentioned previously, particles in quantum mechanics are governed
> by a wave equation, Schrödinger’s equation. Before we look at
> particles as described by quantum physics, let us derive the wave
> equation that describes wave phenomena within classical physics.
> Similar to the equations we have solved up to this point, the wave
> equation is a second order linear differential equation.
>
> **Deriving the wave equation**
>
> First let us consider a string, as illustrated in the figure (1), with
> tension $T$ and mass per unit length$\ \mu$. For the sake of this
> derivation, we will assume that the string extends infinitely in both
> directions. Let’s examine small transverse displacements of the
> string. The coordinate along the string we will call $x$, and the
> transverse displacement $\psi$. Restricting this case to small
> displacements or vibrations means that the angle $\theta$ between the
> string and the $x$ direction is much smaller than one. Therefore we
> can use the small-angle approximation;$\sin(\theta) \approx \theta$
> and $\cos(\theta) \approx \theta$.

![](media/image5.gif){width="3.057292213473316in"
height="1.5202471566054243in"}

> Figure (1) \[3\]

Let’s start by writing the transverse Newton’s second law equation

$F_{\psi} = ma_{\psi}$ (8)

The forces acting in the $\psi\ $direction are

$F_{\psi}$ = $T\sin\theta_{2} - T\sin\theta_{1}$. (9)

Using the small-angle approximation,
$\sin\theta \approx \tan\theta = \frac{d\psi}{\text{dx}},$ so (9)
becomes

$F_{\psi} = T{\{(\frac{d\psi}{\text{dx}})}_{2} - {(\frac{d\psi}{\text{dx}})}_{1}\}.$
(10)

> We can see now that the total force acting in the transverse direction
> is dependent on the difference in slope between the two ends of the
> string. On the right hand side of equation (8) we have mass and
> acceleration. We know $\mu$ is the mass per unit length, therefore the
> mass $dm = \mu\text{dx.\ }$The acceleration in the transverse
> direction is the rate of change in the $\psi$ direction. This is
> simply the second time derivative of $\psi,$ so we have
>
> $F_{\psi} = T{\{(\frac{d\psi}{\text{dx}})}_{2} - {(\frac{d\psi}{\text{dx}})}_{1}\} = \mu\text{dx\ }\frac{d^{2}\psi}{dt^{2}}\text{.\ }$
> (11)
>
> Rearranging to get the $\text{dx}$ terms on one side gives
>
> $\frac{d^{2}\psi}{dt^{2}} = \frac{T}{\mu}\frac{(\frac{d\psi}{\text{dx}})_{2} - (\frac{d\psi}{\text{dx}})_{1}}{\text{dx}}$
> (12)
>
> The numerator of the last term on the right hand side of (12) is the
> difference between the derivatives at points $x$ and $x + dx$, denoted
> by the subscripts 1 and 2 respectively. This numerator is being
> divided by $\text{dx}$, so this term is essentially the rate of change
> of the first derivative with respect to $\text{x.}$ In other words:
> The second derivative of $\psi$ with respect to $x$.
>
> So we now have
>
> $\frac{d^{2}\psi}{dt^{2}} = \frac{T}{\mu}\frac{d^{2}\psi}{dx^{2}}.$
> (13)
>
> $\psi$ is a function of position and time, so we should write $\psi$
> as $\psi(x,t)$. Consequently, we must now use partial derivatives
> since we have a function of two variables so (13) becomes
>
> $\frac{\partial^{2}\psi(x,t)}{\partial t^{2}} = \frac{T}{\mu}\frac{\partial^{2}\psi(x,t)}{\partial x^{2}}$
> (14)
>
> This is the wave equation!
>
> The solutions for the wave equation are in the form
>
> $\psi(x,t) = Ae^{i( \pm kx \pm \omega t)}$ where
> $\frac{\omega}{k} = \equiv c$. (15)
>
> We can find the relationship between $\omega$ and $k$ by substituting
> (15) into the wave equation and subsequently cancelling the
> exponential term. We will get
>
> $- \omega^{2} = - \frac{T}{\mu}k^{2}$ (16)
>
> Which simplifies to
>
> $\frac{\omega}{k} =$ where $\equiv$$c$ (17)
>
> $c$ is the speed of the wave and $\text{k\ }$and $\omega$ can take any
> value as long as they satisfy the relationship $\frac{w}{k} = c$.
> Wavelength is $\lambda = \frac{2\pi}{k}$ and the period of the
> oscillation is$\tau =$$\frac{2\pi}{\omega}\text{\ .\ \ \ }$
>
> **Boundary behaviour and boundary conditions.**
>
> When a wave reaches a boundary, different outcomes will occur
> depending on the boundary. For our purpose, understanding quantum
> tunneling, we will look specifically at waves with two fixed ends and
> waves on a string with a change in density. Understanding the wave
> functions and wave behaviour with these two cases will be very useful
> to us in later sections.
>
> **Reflection and transmission:**
>
> If a string changes density at the point $x = 0$, this point will act
> as a boundary. At $x = 0\ $the incident wave travelling through the
> string will undergo reflection and transmission. As we will discuss
> later, the same occurs with regards to quantum physics when a particle
> encounters a boundary in the form of potential change.
>
> Consider an infinite string with uniform tension but changing density:
> $\mu_{1}$for $- \infty < x < 0$ and $\mu_{2}$for $0 < x < \infty$.
> Given this property, $x = 0$ can be considered as a boundary which a
> wave travelling through the string will encounter. Let’s say a wave of
> the form
>
> $\psi_{i}(x,t) = f_{i}(t -$$\frac{x}{\nu_{1}})$ (18)
>
> (i stands for incident) starts at the left and travels towards
> $x = 0$. Equation (15) tells us that $\nu_{1} =$ At the boundary,
> $x = 0,$ there will be a reflected (r) wave and transmitted (t) wave.
>
> Reflected wave: $\psi_{r}(x,t) = f_{r}(t + \frac{x}{\nu_{1}})$. (19)
>
> This wave moves leftwards, towards $- \infty$ and therefore has a
> positive sign in its argument.
>
> Transmitted wave:
> $\psi_{\text{t\ }}(x,t) = f_{t}(t - \frac{x}{\nu_{2}})$ where
> $\nu_{2} =$ (20)
>
> This wave moves to the right, towards $\infty.$
>
> Now if we were to look at the resultant expressions for the waves on
> the left (L) and right (R) of $x = 0$ we can write
>
> $\psi_{L}(x,t) = \psi_{i}(x,t)\  + \psi_{r}(x,t)\  =$$f_{i}(t -$$\frac{x}{\nu_{1}}) +$$f_{r}(t + \frac{x}{\nu_{1}}$)
>
> $\psi_{R}(x,t) = \psi_{t}(x,t)\  =$$f_{t}(t -$$\frac{x}{\nu_{2}}).$
> (21)
>
> We have three different wave functions here, but if we find the
> reflected and transmitted waves in terms of the incident wave, we can
> simplify equation (21) to obtain a complete wave function that we can
> understand further. This can be done using the *boundary conditions*
> at $x = 0$.
>
> Condition 1: The string is continuous therefore
>
> $\psi_{L}(0,t) = \psi_{R}(0,t)$⇒ $f_{i}(t) + f_{r}(t) = f_{t}(t)$.
> (22)
>
> Condition 2: The slope is continuous. If there was a difference in
> slope between the left and right side of $x = 0$ it would imply that
> there is a resultant force acting on the atom at $x = 0$. But a
> nonzero force implies that acceleration, $a = \frac{F}{\mu\text{dx}},$
> would be infinite since we are taking $\text{dx}$ to be infinitesimal.
> Since this is not possible, the slope must be constant and therefore
>
> $\frac{\partial\psi_{L}(x,t)}{\partial x}$=
> $\frac{\partial\psi_{R}(x,t)}{\partial x}$ ⇒
> $- \frac{1}{\nu_{1}}{f^{'}}_{i}(t) +$$\frac{1}{\nu_{1}}{f^{'}}_{r}(t) = - \frac{1}{\nu_{2}}{f^{'}}_{t}(t).$
> (23)
>
> Integrating and rearranging to remove the fractions we get
>
> ${\nu_{2}\text{\ f}_{i}(t) - \nu_{2}\text{\ f}_{r}(t) = \nu_{1}\ f_{t}(t)}_{.}$
> (24)
>
> We will assume the string has zero displacement before the wave passes
> so we do not need to consider an integration constant.
>
> Now we can find the relationships between both$\text{\ f}_{r}(t)$and
> $f_{t}(t),$ and $\text{\ f}_{i}(t)$ by solving equations (22) and
> (24). We get
>
> $\text{\ f}_{r}(t) = \frac{\nu_{2} - \nu_{1}}{\nu_{2} + \nu_{1}}$$f_{i}(t)$
> and
> $\text{\ f}_{t}(t) = \frac{2\nu_{2}}{\nu_{2} + \nu_{1}}$$\text{\ f}_{i}(t),$
> (25)
>
> We have written $t$ as the argument of the functions here but this
> relationship holds true regardless of the argument. So we can rewrite
> (21), the full wave, as
>
> $\psi_{L}(x,t) = \psi_{i}(x,t)\  + \psi_{r}(x,t)\  =$$f_{i}(t -$$\frac{x}{\nu_{1}}) +$$\frac{\nu_{2} - \nu_{1}}{\nu_{2} + \nu_{1}}f_{i}(t + \frac{x}{\nu_{1}}$)
>
> $\psi_{R}(x,t) = \psi_{t}(x,t)\  =$${\frac{2v_{2}}{v_{2} + v_{1}}f}_{i}(t -$$\frac{x}{\nu_{2}}).$
> (26)
>
> *Reflection and transmission coefficients:*
>
> Reflection and transmission coefficients ($R$ and $T,$ respectively)
> represent what amount of the incident wave is reflected/transmitted.
>
> What we can infer from (25) is the reflection and transmission
> coefficients. They are simply the coefficients of $f_{i}(t),$ the
> amplitudes of the reflected and transmitted waves relative to the
> incident wave. So the reflection and transmission coefficients are
>
> $R \equiv \frac{\nu_{2} - \nu_{1}}{\nu_{2} + \nu_{1}}\ $and
> $T \equiv \frac{2\nu_{2}}{\nu_{2} + \nu_{1}},$ respectively. (27)
>
> Note that the coefficients must always satisfy the relation
> $1 + R = T.$
>
> To look at the cases involving a change in density in a string, it
> will be useful to bring in the variable $\mu$ into our analysis so
> that the boundaries can be clearly represented by the density, or
> change in density.
>
> We know that $\nu =$ and that the tension $T$ of the string remains
> constant. Therefore $\nu_{1} \propto \frac{1}{}$ and
> $\nu_{2} \propto \frac{1}{}$. With this, we can write $R$ and $T$ in
> terms of the densities $\mu_{1}$and $\mu_{2}$:
>
> $R \equiv \frac{-}{+}$ and $T \equiv \frac{2}{+}$ (28)
>
> Now let's look at applications of the formulas we have derived to
> different cases involving density change:

1.  *Light string on left, heavy string on right:*
    > $\mu_{1} < \mu_{2} < \infty$ ($\nu_{2} < \nu_{1})$ ⇒
    > $- 1 < R < 0,\ 0 < T < 1.$

> We have already discussed it in this section; both reflection and
> transmission will occur once the wave reaches the heavy side of the
> string. Note that R is negative which means that the wave will be
> inverted as it moves back to the left. This happens for the following
> reason: As the wave reaches $x = 0$, the end of the waves on the left
> and right exert upwards and downwards forces, respectively. This is
> explained by Newton’s third law that ‘for every action there is an
> equal and opposite reaction.’ Due to the greater density on the right
> side relative to the left, the upward force becomes a downward force
> “causing the upward displacement to become downward displacement,
> hence the inverted reflected wave.” \[4\]

1.  *Heavy string on left, light string on right:*
    > $0 < \mu_{2} < \mu_{1}\ (\nu_{1} < \nu_{2})$⇒
    > $0 < R < 1,\ 1 < T < 2.$

> This case is similar to case 1 as there is partial reflection and
> partial transmission. However in this case there will be more
> transmission than reflection. It is also worth noting that the
> reflection coefficient is positive, therefore the reflected wave is
> not inverted.

1.  *Zero mass string on the right:* $\mu_{2} = 0\ (\nu_{2} = \infty)$⇒
    > $R = 1,\ T = 2.$

> Since the right part of the string is massless, it cannot carry any
> energy. Therefore the wave is completely reflected. However, there is
> no inversion of the reflected wave since the zero-mass string will not
> exert any downward force on the string.

1.  *Brick wall on the right:* $\mu_{2} = \infty$ ($\nu_{2} = 0$) ⇒
    > $R = \  - 1,\ T = 0\ .$

> No part of the wave will be transmitted, meaning that all of the wave
> is reflected. However $R$ is negative which means that the wave will
> be inverted as it moves back to the left. As the wave reaches the
> wall, the string experiences a downwards force. Since energy must be
> conserved and the wall cannot absorb any energy being infinitely
> massive, the wave ends up inverted.
>
> **Standing waves**
>
> We have used the boundary conditions at $x = 0$ but what if we require
> that the wave function satisfies the condition
> $\psi(0,t) = \psi(L,t) = 0?$ What sort of wave function would we get?
>
> Let us look back at the brick-wall case in more detail. We will decide
> that the wall is located at $x = 0.$ First, the general solution for
> the wave equation from (15) is
>
> $\psi(x,t) = e^{i(kx + \omega t)}.$
>
> Consider a sinusoidal wave moving towards the left where it will be
> incident on the wall. We can take the real part of the above function,
> which gives
>
> $\psi_{i}(x,t) = \cos(\omega t + kx).$ (29)
>
> As we discovered previously, the reflection coefficient of $\psi(x,t)$
> when it encounters a wall is $- 1$. So the reflected wave that travels
> in the opposite direction is
>
> $\psi_{r}(x,t) = - \cos(\omega t - kx).$ (30)
>
> So the total wave is
>
> $\psi(x,t) =$$\psi_{i}(x,t)$+$\psi_{r}(x,t) =$$\cos(\omega t + kx)$$- \cos(\omega t - kx)$
>
> $= - 2\sin(\omega t)\sin\text{kx.}$ (31)
>
> Equation (31) satisfies the first boundary condition $\psi(0,t).$ As
> we can see, the total wave function is made up of a product of a
> function of $x$ and a function of $\text{t.}$ This is a standing wave.
> All points on the string will be at rest at exactly the same times,
> unlike travelling waves where the peaks and troughs are
> instantaneously at rest.
>
> We now need to consider the second boundary condition:
> $\psi(L,t) = 0.$ If we substitute $x = L\ $into equation (31), the
> condition would only be satisfied if $\sin(kL) = 0.$ Hence $kL = n\pi$
> where $n$ is an integer, giving

$k_{n} = \frac{n\pi}{L}$.

> The method we have gone through is relevant to quantum tunneling. Here
> we have looked at $\psi(0,t) = \psi(L,t) = 0,$ which gives a standing
> wave within two fixed ends, but in quantum mechanics this is the same
> condition that arises when there is an infinite potential barrier.
>
> **Attenuation**
>
> In quantum tunneling, the wave function in the area of high potential
> energy (i.e within the barrier) takes a decaying exponential form. How
> does this happen? To understand, let us look at our classical system
> and explore what happens when a string experiences *attenuation,*
> which causes $\psi(x,t)$ to decay. Attenuation can occur when a string
> experiences an additional force such as drag force from damping if it
> were submerged underwater. Here we will explore a different case in
> which the string, instead of vibrating freely, is attached to a bed of
> springs, which will add an additional force.
>
> When there are no springs, the wave equation from equation (15) is
>
> $\frac{\partial^{2}\psi(x,t)}{\partial t^{2}} = \frac{T}{\mu}\frac{\partial^{2}\psi(x,t)}{\partial x^{2}}.$
>
> To incorporate the additional force from the springs, let's get this
> equation into a more familiar form. If we multiply through by the
> length of a bit of string $\Delta x$ and rearrange we can obtain the
> $F = ma$ equation
>
> $T\Delta x\frac{\partial^{2}\psi}{dx^{2}} = \mu\Delta x\frac{\partial^{2}\psi}{dt^{2}}$.
> (27)
>
> Now let’s add the force from the springs. Take $\sigma$ to be the
> spring constant per unit length. The spring constant is therefore
> $\sigma\Delta\text{x.}$ The force on a spring is $F = - kx,$ so the
> force from the bed of springs is

$F = - \sigma\Delta x\psi$. (28)

Placing this appropriately into (27) gives

> $T\Delta x\frac{\partial^{2}\psi}{dx^{2}} - \sigma\Delta x\psi = \mu\Delta x\frac{\partial^{2}\psi}{dt^{2}}.$
> (29)
>
> If we divide the equation by $\Delta x$ we will get a differential
> equation for $\psi(x,t).$ To solve it let’s substitute
>
> $\psi(x,t) = e^{i(kx - \omega t)}.$ (30)
>
> This will give the relationship between $\omega$ and $k,$ which comes
> out as
>
> $- Tk^{2}e^{i(kx - wt)} - \sigma e^{i(kx - wt)} = - \mu\omega^{2}e^{i(kx - wt)}.$
> (31)
>
> Now let’s cancel out the exponential term and solve for $k$. We get
>
> $- Tk^{2} - \sigma = - \mu\omega^{2}.$ (32)
>
> Solving gives
>
> $k = \pm$. (33)
>
> Depending on whether the discriminant $\mu\omega^{2} - \sigma$ is
> positive or negative, $k$ can take a real or imaginary value. If
> $\mu\omega^{2} < \sigma$, $k$ is imaginary and if
> $\mu\omega^{2} > \sigma$, $k$ is real. It can also take the positive
> or negative value of the square root. The question now is which value
> of $k$ should we use? For now, we will use the positive and imaginary
> value.
>
> Lets define
>
> $k = i\kappa$, where $\kappa$ is real. (34)
>
> If we substitute this into (30) we get
>
> $\psi(x,t) = e^{i(i\kappa x - \omega t)}.$ (35)
>
> Expanding the power of $e$ then gives
>
> $\psi(x,t) = e^{- \kappa x - i\omega t}.$ (36)
>
> Looking carefully at the above function, we can see that $x$ is now
> being multiplied by a negative factor: $- \kappa$. This shows us that
> $\psi(x,t)$ decays with distance. The envelope of the function as it
> decays is equal to $\psi(x,t) = e^{- \kappa x}.$ This wave can now be
> classified as an attenuated wave because it narrows as $x$ grows.
>
> Now we can also see why taking the positive value of $k$ is necessary,
> if we took the negative value, $x$ in the function for $\psi(x,t)$
> would be multiplied by a positive factor, $\kappa$. Instead of
> decaying, the wave function would increase with time, which is not
> possible since the string doesn’t have the source of energy to account
> for this behavior.
>
> **2.2 Symmetry and conservation**
>
> The final concept from classical physics that will be useful to us
> comes from Noether’s Theorem, which states that ‘*every symmetry of a
> system gives rise to a dynamically conserved quantity*.’ This means
> that the conservation laws can be related with a symmetry of a certain
> system.
>
> Let us look at how the above statement is true for momentum. We will
> begin with the question: *When is momentum conserved?* We can use
> Newton’s second law and find an equation involving momentum for a ball
> being thrown. We have
>
> $F = ma.$ (37)
>
> Since acceleration is the rate of change in velocity with respect to
> time, giving
>
> $F = m\frac{\text{dv}}{\text{dt}}.$ (38)
>
> Assuming the mass of the ball stays constant we can write
>
> $F = \frac{d}{\text{dt}}(mv).$ (39)
>
> Momentum is equal to $\text{mv}$ so
>
> $F = \frac{\text{dp}}{\text{dt}}.$ (40)
>
> Equation (40) shows us that force is the change of momentum. So the
> answer to the original question is momentum is conserved when the
> force is zero, as there will be no change in momentum over time.
>
> Taking energy to be conserved, let us now find the potential, $V(x)$
> of the system, specifically the amount of potential energy used when
> an object moves from the ground to a certain height.
>
> The equation for the gravitational force is
>
> $F = - mg\widehat{y}.$ (41)
>
> The potential is the work done in taking the object to a certain $y$
> value and work is force times distance. However force is changing over
> time, so we must find the work done by adding the individual values of
> work, which can be represented by the integral
>
> $V(x) = - F({x'}^{})dx'.$ (42)
>
> Because the force is acting against gravity the dot product will be
> negative, but since we want a positive answer we put a negative sign
> in front of the integral.

Now let’s take the derivative of equation (42). We get

$\frac{\text{dV}}{\text{dx}} = - F(x).$ (43)

> Since we have taken $F(x)$ to be zero we can see using (43) that when
> force is zero, the potential should be constant with position in the
> $x$ direction. This means that if the system was shifted to the left
> or right, the potential would be the same. In other words, there is
> *symmetry of translation.* Note that equation (43) is a general
> representation, as the use of gravity here is just an example.

To summarise, we now have

$\frac{\text{dp}}{\text{dt}} = 0 = F(x) = - \frac{\text{dV}}{\text{dx}}.$
(44)

> This aligns with Noether’s theorem as it shows that the conserved
> quantity (momentum) corresponds to a symmetry (translation). The same
> relation holds true for energy and time translation as well as angular
> momentum and rotation.
>
> **3. Schrödinger’s Wave Equation**

**3.1 Deriving Schrödinger’s Equation starting from Symmetry and
Conservation.**

> Now we transition to quantum mechanics. As mentioned previously,
> particles as described by quantum physics act like waves. The
> wave-like behaviour is represented by Schrödinger’s equation, which
> determines a wavefunction $\psi(x,t).$ To derive Schrödinger’s
> equation we must introduce and use quantum principles. In order to do
> this we can begin with the classical concept of symmetry and
> conservation and see how it relates to quantum mechanics. We can then
> find relationships between conserved quantities, namely energy and
> momentum, using our knowledge of differential equations. Incorporating
> the wavefunction $\psi$ into these relationships, we will be able to
> find Schrödinger’s equation.
>
> First, here is a summary of the symmetry and conservation
> relationships:

          **Momentum ⎼⎼⎼⎼⎼⎼⎼→**            **Translation**
  ------- -------------------------------- -----------------
  Units   $\text{kg\ m\ }s^{- 1}$          $m$
          **Energy ⎼⎼⎼⎼⎼⎼⎼⎼→**             **Time**
  Units   $\text{kg\ }m^{2}\ s^{- 2}$      s
          **Angular Momentum ⎼⎼⎼⎼⎼⎼⎼⎼→**   **Rotation**
  Units   $\text{kg\ }m^{2}\ s^{- 1}$      1 (unitless)

> Angular momentum is not strictly relevant to Schrödinger’s equation,
> but it has been added to make the following observation more clear.
>
> If we multiply the units of the conserved quantity with the units of
> the symmetrical aspect of the system, we get the exact same units
> $\text{kg}\text{\ m}^{2}\text{\ s}^{- 1}.$ This now leads us to an a
> connection to quantum physics as these units are also the units of an
> important constant: Planck’s constant, $\text{h.}$ In 1900 Max Planck
> was trying to find the spectrum of colours emitted by a thermal
> radiator. The results couldn’t be explained by the existing physics at
> the time, so Planck postulated that energy of light must come in
> packets called quanta, and that the energy is proportional to the
> light’s frequency by the constant $h,$ now known as Planck’s constant.
> By dimensional analysis, it could be found that this constant of
> proportionality has these same units,
> $\text{kg}\text{\ m}^{2}\text{\ s}^{- 1}.$ Its value is
> $6.62607015\  \times \ 10^{34}\text{\ kg}\text{\ m}^{2}\text{\ s}^{- 1}.$
> This constant is important to quantum physics.
>
> To derive Schrödinger’s equation let’s look back at the solution to
> the wave equation from section 2. The function is
>
> $\psi(x,t) = {e^{i(kx - \omega t)}.}^{}$ (1)
>
> We can use Planck’s constant
>
> $h = 6.62607015\  \times \ 10^{34}\text{\ kg}\text{\ m}^{2}\text{\ s}^{- 1}$
> (2)
>
> to generate a relationship from (1) between $\omega$and energy because
> it relates a photon's energy to its frequency. Using Planck’s constant
> we can write
>
> $E = hf.$ (3)

Multiplying and dividing the RHS by $2\pi$ gives

$E = \frac{h}{2\pi} \cdot 2\pi\text{f.}$ (4)

> We define $\frac{h}{2\pi} = \hslash$ and $2\pi f = \omega,$ so we now
> have an equation relating angular frequency and energy as

$E = \hslash\omega.$ (5)

> Now let’s see how we can find a relationship between equation (1) and
> (5) so that we involve $\psi$. If we took the first derivative with
> time, we would bring down $\omega$ from the power. But it also brings
> down $- i.$ Furthermore, it doesn’t involve $\hslash.$ However, if we
> multiplied the first derivative by $i$ and $\hslash,$ we would get
>
> $i\hslash\frac{\partial}{\partial t}\psi = \hslash\omega\psi = E\psi.$
> (6)
>
> This links back to Noether’s theorem as the time derivative gives us
> the energy. This would suggest that the $x$ derivative will give you
> momentum. We can begin by writing

$\frac{\partial}{\partial x}\psi$\~ $p\psi$ (7)

> The derivative of $\psi(x,t)$ with respect to $x$ is actually
>
> $\frac{\partial}{\partial x}\psi = ik\psi.$ (8)
>
> The units for momentum are $\text{kg}\text{ms}^{- 1},$ but the unit
> for $k$ is just $m^{- 1}.$ Therefore we need to multiply the
> derivative by some constant with the units $\text{kg}m^{2}s^{- 1}.$ As
> we discovered, $\hslash$ has these exact units. So we can modify (7)
> to
>
> $\hslash\frac{\partial}{\partial x}\psi\ $\~ $p\psi.$ (9)
>
> Since we prefer not to have an $i$, we can multiply the LHS of (9) by
> $- i,$ which gives us a more definitive equation
>
> $- i\hslash\frac{\partial}{\partial x}\psi$$= \widehat{p}\psi.$ (10)
>
> Here we have derived an equation that works when
> $\psi(x,t) = {e^{i(kx - \omega t)}.}^{}$However, there are many
> different possible functions which we need the equation to account for
> so that we can find their momentum as well. If we consider $p$ not
> simply as the classical quantity momentum but rather as the act of
> multiplying $\psi$ by $- i\hslash\frac{\partial}{\partial x}$, it
> becomes more widely usable. The concept of doing something to a
> function in mathematics is called an operator, where the operator is
> marked with a ‘hat’. Going forward when we derive Schrödinger’s
> equation we will be exchanging numbers for operators, eventually
> deriving an equation of operators.

Now we have an equation for both energy and momentum in terms of $\psi.$

To bring it all together, we can find an equation to relate energy and
momentum.

Energy can be defined as

$E = KE + PE.$ (10)

$KE = \frac{1}{2}mv^{2}$ and $p = mv$ (11)

Therefore

$KE = \frac{1}{2}mv^{2} = \frac{p^{2}}{2m}.$ (12)

We can substitute this into (10) to get

$E = \frac{p^{2}}{2m} + V(x).$ (13)

> Let us assume equations (6) and (10) are true at the same time and see
> what we can get for the wavefunction. Multiplying both of equation
> (13) by $\psi$ gives

$E\psi = \{\frac{p^{2}}{2m} + V(x)\}\psi.$

> Now, instead of continuing to solve the equation with the classical
> quantities $p$ and $E,$ we are going to do something different. That
> is *replacing the classical quantities by their operators*. We will
> replace the quantity $p$ by the value of the $\widehat{p}$ operator we
> found in equation (6). For $E$ we will substitute by the operator
> suggested in equation (10). In doing this we get

$i\hslash\frac{\partial}{\partial t}\psi = \frac{( - i\hslash)^{2}\frac{\partial^{2}\psi}{\partial x^{2}}^{}}{2m} + V(x)\psi.$
(14)

Expanding gives

$i\hslash\frac{\partial}{\partial t}\psi = \frac{- \hslash^{2}}{2m}\frac{\partial^{2}\psi}{\partial x^{2}} + V(x)\psi$.
(15)

This is Schrödinger’s equation! More specifically, it is the
time-dependent Schrödinger equation.

> As we have seen, the Schrödinger equation is linked to equation (13)
> $E = \frac{p^{2}}{2m} + V(x),\ $which is based on classical mechanics.
> This equation can be extended to include the classical Hamiltonian
> function $H(p_{x},x)$ by writing it as
>
> $E = KE(p_{x}) + V(x) = H(p_{x},x).$ (16)
>
> Now replacing $p_{x}$ by the operator found in (10) and $E$ with the
> operator found in (6), we get
>
> $\widehat{H}$$( - i\hslash\frac{\partial}{\partial x},x)\psi =$$- \frac{\hslash^{2}}{2m}\frac{\partial^{2}\psi}{\partial x^{2}} + V(x)\psi = i\hslash\frac{\partial}{\partial t}\psi.$
> (17)
>
> This is identical to equation (15), but we can now see that the wave
> equation can be written as
>
> $\widehat{H}\psi = i\hslash\frac{\partial}{\partial t}\psi.$ (18)
>
> **3.2 Solving Schrödinger’s equation**
>
> **The Time-Independent Equation**
>
> Let us now look at how to solve Schrödinger’s equation (15). As we
> have done in previous sections with partial differential equations, we
> will first deal with the solutions of $\psi.$ We can attempt to
> express the wavefunctions as the product of two function; one
> involving time alone and the other only involving the coordinate:
>
> $\Psi(x,t) = \psi(x)\varphi(t).$ (19)
>
> Rewriting Schrödinger’s equation with this and dividing through by
> $\psi(x)\varphi(t)$ gives
>
> $\frac{1}{\psi(x)}\left\{ - \frac{\hslash^{2}}{2m}\frac{d^{2}\psi(x)}{dx^{2}} + V(x)\psi(x) \right\} =$$i\hslash \cdot \frac{1}{\varphi(t)}\frac{d\varphi(t)}{\text{dt}},$
> (20)
>
> where the right-hand side is a function of time alone and the left
> side is a function of the position alone. Consequently, both of the
> sides must be equal to a constant, since it is the only quantity that
> is independent of $x$ and $\text{t.}$ We will call this constant
> $\text{E.}$ We can now write equation (20) as two equations. We have
>
> $\frac{d\varphi(t)}{\text{dt}} = \ \frac{- i}{\hslash}E\varphi(t)$
> (21)
>
> and
>
> $- \frac{\hslash^{2}}{2m}\frac{d^{2}\psi(x)}{dx^{2}} + V(x)\psi(x) = E\psi(x),$
> (22)

which can also be written as

$\frac{d^{2}\psi}{dx^{2}} + \frac{2m}{\hslash^{2}}(E - V(x))\psi = 0.$
(23)

> Equation (23) is generally known as the time-independent Schrödinger’s
> equation, or the amplitude equation since the position function
> $\psi(x)\ $determines the amplitude of the $\Psi(x,t).$ The equation
> provides a number of solutions that correspond to various values of
> $\text{E.}$ These values can be represented with the subscript
> $\text{n.}$ Consequently we will denote the corresponding functions as
> $\psi_{n}(x).$ The corresponding time function, $\varphi(t)$ can be
> integrated to give
>
> $\varphi_{n}(t) = e^{- iE_{n}t/\hslash}.$ (24)
>
> The general solution of Schrödinger’s equation will be the sum of all
> $n$ solutions. So the general expression for the wave function can be
> written as
>
> $\Psi(x,t) = a_{n}\Psi_{n}(x,t) = a_{n}\psi_{n}(x)e^{- iE_{n}t/\hslash},$
> where $a_{n}$ denotes an arbitrary coefficient. (25)
>
> We will find later that the constant $E_{n}$ is required to represent
> the energy of various stationary states of the system.
>
> Equation (25) contains the unknowns $\psi_{n}(x)$ and $E_{n}$ for
> which we need to find values for. The functions $\psi_{n}(x)$ that
> satisfy Schrödinger's equation, equation (23), are called
> wavefunctions or *eigenfunctions*. These wavefunctions exist for
> certain values of $E_{n}.$ These certain values are the
> “characteristic energy values or *eigenvalues* of the wave equation”
> (Pauling). A wavefunction must have certain properties in order to be
> considered a satisfactory solution of Schrödinger’s equation. The
> wavefunction must be:

1.  Continuous

2.  Single valued

3.  Finite for all values of $\text{x.}$

> The eigenvalues $E_{n}$ can occur as a set of only discrete values, or
> as a set of continuous values, or as both.
>
> In order to find $\psi_{n}(x)$ and $E_{n}$ for equation (25), we can
> use the time-independent Schrödinger's equation - equation (23). Since
> it is a second order differential equation, we are familiar with the
> method used to solve it.
>
> **Solving the Time-Independent Schrödinger’s Equation**
>
> Let’s take the example of a particle within an infinite potential well
> given by
>
> ![](media/image1.png){width="1.578125546806649in"
> height="0.4508923884514436in"}
>
> Since the potential is infinite beyond $L/2,$ we have the boundary
> condition $\psi( \pm L/2) = 0.$ Now we will split the system into
> three regions - the left, right and middle regions which we will call
> regions I, II and III respectively. They will each have different
> time-independent Schrödinger equations. For our purpose, we will just
> look at the equation for region II:
>
> Region II:
> $- \frac{L}{2} \leq x \leq \frac{L}{2}\ \  \Rightarrow \ \frac{d^{2}\psi}{dx^{2}} + \frac{2m}{\hslash^{2}} \cdot E\psi = 0.$
> (26)
>
> Position-wise, region II describes the middle of the potential well,
> so we will just write $E\psi$ since the potential between
> $- \frac{L}{2}$ and $\frac{L}{2}$ is zero. Looking at equation (26),
> we can see that it will be easier to solve for $\psi$ and $E$ if we
> let
>
> $k =$
>
> Now equation (26) looks like
>
> $\frac{d^{2}\psi}{dx^{2}} + k^{2}\psi = 0$ (27)
>
> which now more closely resembles the second differential equations we
> have solved in previous sections. Since the second derivative of
> $\psi$ is equal to its negative multiplied by $k^{2},$ we can deduce
> that $\psi$ could be the complex exponential
>
> $\psi = e^{\pm ikx},$ (28)
>
> In its full trigonometric form, (28) becomes
>
> $\psi = A\cos kx + B\sin kx,$ where $A = C_{1} + C_{2}\ $and
> $B = C_{1} - C_{2}.$ (29)
>
> In order to find the value of $k,$ we will need to utilise the
> boundary conditions. Substituting the values $x = \frac{L}{2}$ and
> $x = - \frac{L}{2}$ and equating to zero gives the expressions
>
> $\psi(\frac{L}{2}) = A\cos\frac{\text{kL}}{2} + B\sin\frac{\text{kL}}{2} = 0,$
> (30)
>
> $\psi( - \frac{L}{2}) = A\cos\frac{\text{kL}}{2} - B\sin\frac{\text{kL}}{2} = 0.$
> (31)
>
> Solving equations (30) and (31) simultaneously gives the following two
> possibilities:
>
> $2A\cos\frac{\text{kL}}{2} = 0,\ B = 0$ (32)
>
> or
>
> $2B\sin\frac{\text{kL}}{2} = 0,\ A = 0.$ (33)
>
> So we have two sets of values for $\text{k.}$ Let’s solve (32) and
> (33) to see what type of values we get. Solving (32) gives
>
> $\frac{\text{kL}}{2} = \pi(n + \frac{1}{2})$ where $n$ is any integer
>
> and solving (33) gives
>
> $\frac{\text{kL}}{2} = \pi\text{n.}$
>
> This tells us that $k$ has discrete values. We can then infer that
> there are discrete energy $E$ values corresponding to the wavefunction
> solutions since $E_{n}$\~ $\text{k.}$ For each of the energy values or
> eigenvalues $E$ there will be a wavefunction/eigenfunction containing
> the value $\text{E.}$ These fixed values of energy tell us that the
> oscillation of the particle in region II is uniform. As defined
> previously, $E = hf,$ so the frequency is also fixed. So, these
> solutions, or eigenfunctions are also called stationary states, as the
> energy for each solution is fixed. This is how we solve the
> time-independent Schrödinger equation, and its results allow us to
> solve the full Schrödinger equation (equation (25)).
>
> For visual reference, here are rough diagrams showing the graph forms
> for the wavefunctions for the first few values of $n$:
>
> ![](media/image4.png){width="1.72753280839895in"
> height="1.578125546806649in"}![](media/image8.png){width="1.9583333333333333in"
> height="1.665313867016623in"}![](media/image6.png){width="2.15625in"
> height="1.7694805336832895in"}
>
> ![](media/image7.png){width="2.6145833333333335in"
> height="1.8802088801399826in"}
>
> Figure 1
>
> Note that the diagrams are rough and that these graphs actually have
> equal amplitudes. However as $n$ increases by 1, the same scale fits
> another half wavelength. As time changes, these graphs will oscillate
> up and down, keeping their exact form.
>
> **Significance of the Wavefunctions/Eigenfunctions**
>
> Wavefunctions are useful because they are directly linked to
> probability. Specifically, *the square of a wavefunction is
> proportional to the “probability of finding the particle at a given
> point and time”* \[6\].
>
> Looking back at the boundary condition from the infinite well problem
> we see that the condition$\psi( \pm L/2) = 0$ must be satisfied since
> the particle cannot enter the area where potential is infinite. The
> wavefunction is equal to zero because the probability of the particle
> existing at $x = \pm L/2$ is also zero.
>
> The complex conjugate of $\Psi(x,t)$ is the wavefunction
> $\Psi^{*}(x,t).$ Let us consider the product of a solution $\Psi(x,t)$
> and its conjugate $\Psi^{*}(x,t).$ This function,
> $\Psi(x,t)\Psi^{*}(x,t)$ is real and defined for all $x$ values from
> $- \infty$ through to $+ \infty$. We can postulate that the quantity
> $\Psi(x,t)\Psi^{*}(x,t)$is the *probability distribution function for
> the system.* $\Psi(x,t)\Psi^{*}(x,t)dx$ can therefore be used to
> represent the probability that the particle is in “the region between
> $x$ and $x + dx$ at the time $t$” \[5\]. The probability density can
> also be written as $\left| \psi(x) \right|^{2}.$

**4. Quantum Tunneling**

> **Solving One-Dimensional Quantum Problems: Barrier tunneling**
>
> Now that we have gone through solving second order differential
> equations, classical wave concepts and Schrödinger's equation, we can
> finally look at how to solve the quantum problem of a particle
> tunneling through a potential barrier!
>
> We looked at reflection and transmission at boundaries for classic
> waves. Since particles behave like waves, we can apply the same ideas
> about transmission and reflection to particles. Previously we
> discussed the boundaries being points on a string at which the string
> mass changes. In the case of particles, the boundaries are the
> positions where the potential changes. At these points there could be
> transmission and/or reflection. It acts similar to light going through
> a medium.
>
> Unlike classical physics however, we have the possibility of quantum
> tunneling, where a particle penetrates a potential barrier to reach a
> classically inaccessible reigon. The probability of the particle
> existing in this third region decays, but doesn’t reach zero. Although
> the region is classically inaccessible, we will find that the behavior
> of the particle in quantum mechanics is analogous to attenuation in
> classical physics; a system we looked at in section two in which there
> is a mechanism for energy dissipation.
>
> Tunneling is possible when the “region where $V > E$ is only of finite
> extent,” in which case “a particle may ‘leak’ through a potential
> barrier” \[Bohm\]. Now let’s look at the tunneling problem. We will
> take the potential
>
> ![](media/image2.png){width="1.6510422134733158in"
> height="0.4269936570428696in"}
>
> We will consider particles coming in from the left with $E < V_{0}.$
> Using the information given, we can represent the potential in three
> different regions with figure 1.
>
> Figure 1
>
> It is worth noting that the potential represented in Figure 1 is
> called a ‘square potential’ because of the 90 degree corners in the
> graph, however this type of potential is an approximation. In nature
> there wouldn't be square potentials as that would “imply an infinite
> force at the points of discontinuity in the potential.” However, these
> graphs do help us illustrate actual systems with enough accuracy.
>
> Now that we have our system set up, we want to find the *probability
> that particles tunnel* through to region three. Because of the wave
> nature of matter, there is a probability of transmission through the
> barrier and penetration of the boundary at $x = L.$ The probability of
> tunneling is equal to the ratio of the rate of outgoing particles to
> incoming particles. Once we find the coefficients of the waves at each
> region, we will be able to solve for the transmission coefficient,
> $\text{T.}$ So we first need to find out the solutions for each
> region’s Schrödinger equation.
>
> First let’s write the time independent Schrödinger equation for each
> region as we did with the infinite well example in section three. We
> have
>
> Region I:
> $x < 0\  \Rightarrow \ \frac{d^{2}\psi}{dx^{2}} = \frac{2m}{\hslash^{2}}( - E)\psi,$
> (1)

Region II:
$0 < x < L\  \Rightarrow \ \frac{d^{2}\psi}{dx^{2}}(V_{0} - E)\psi,$ (2)

Region III:
$x > L\  \Rightarrow \ \frac{d^{2}\psi}{dx^{2}} = \frac{2m}{\hslash^{2}}( - E)\psi.$
(3)

Now let us find the two independent solutions for each of these regions.

> Equations (1), (2) and (3) are all second order differential
> equations. At this point we are more familiar with this form of
> equation. So, we can straight away see that equations (1) and (3) will
> have solutions in the form of complex exponentials since there must be
> an imaginary number in the power for $\psi$ to satisfy the negative
> relationship with its second derivative. Furthermore, solutions to
> equation (2) will be exponentials, but not complex.
>
> For equations (1) and (3) lets define
>
> $k^{2} = \frac{2mE}{\hslash^{2}}$.
>
> So for region I we have
>
> $\psi = Ee^{\pm ikx}$ (4)
>
> which we can then write as two independent solutions
>
> $\psi = De^{\text{ikx}}$

$\psi = Fe^{- ikx}.$ (5)

> Similarly, the independent solutions for region III are
>
> $\psi = \text{Ae}^{\text{ikx}}$

$\psi = A_{1}e^{- ikx}.$ (6)

> For region two, we will define
>
> $\kappa^{2} = \frac{2m(V_{0} - E)}{\hslash^{2}}.$
>
> Now we have the equation
>
> $\frac{d^{2}\psi}{dx^{2}} = \kappa^{2}\psi,$ (7)
>
> which has the two independent solutions
>
> $\psi = \text{Be}^{\kappa x}$

$\psi = Ce^{- \kappa x}.$ (8)

> $A,\ A_{1},\ B,\ C,\ D$ and $F$ are all undetermined coefficients. We
> will leave the solutions as complex exponents for simplicity in the
> consequent steps.
>
> For region III, $x > L,$ we can actually eliminate one of the
> solutions. The wavefunction in region III can only represent
> transmitted particles moving towards the right, as the particles enter
> the first region only from the left. Therefore the solution for region
> III, $\psi = A_{1}e^{- ikx}$ can be rejected as a solution.
>
> Now we can move on to finding the coefficients $A,\ B,\ C,\ D$ and
> $\text{F.}$ We will not be able to find actual values, but we can form
> equations in order to express the coefficients in terms of each other.
> The first two equations we can form come from using two important
> conditions of the wavefunction: $\psi$ and $\frac{d\psi}{\text{dx}}$
> must be continuous at $x = L.$ These are the same conditions that we
> had for the transverse wave on a string. We can now write equations
> relating the solutions of region II and III.

So we have

> $Be^{\kappa L} + Ce^{- \kappa L} = Ae^{\text{ikL}}$ (9)
>
> and
>
> $\kappa Be^{\kappa L} - \kappa Ce^{- \kappa L} = ikAe^{\text{ikL}}.$
> (10)
>
> Solving (9) and (10) simultaneously gives us
>
> $2\kappa Be^{\kappa L} = (\kappa + ik)Ae^{\text{ikL}}.$ (11)
>
> Rearranging for $B$ gives
>
> $B = \frac{(\kappa + ik)}{2\kappa}Ae^{(ik - \kappa)L}.$ (12)
>
> We also get
>
> $2\kappa Ce^{- \kappa L} = (\kappa - ik)Ae^{\text{ikL}}$ (13)
>
> so
>
> $C = \frac{(\kappa - ik)}{2\kappa}Ae^{(\kappa + ik)L}.$ (14)
>
> For a range of parameters, we can actually ignore the smaller of
> $\text{B\ }$and $\text{C.}$ Comparing $\text{B\ }$and $C$ we see that
> the only difference in terms of magnitude is the exponential terms;
> $e^{(ik - \kappa)L}$ and $e^{(\kappa + ik)L}.$ The negative sign in
> the power of the exponential term of $B$ indicates that $C$ must have
> the greater magnitude. The factor $e^{(ik - \kappa)L}$ will be very
> small when either $V_{0}$ is much greater than $E$ or when $L$ is very
> large. So $\text{B\ }$is actually negligible for these range of
> parameters.
>
> Now let us write the equations for continuity of $\psi$ and
> $\frac{d\psi}{\text{dx}}$ at $x = 0$ so that we can find the constants
> $D$ and $F$ in terms of $B$ and $\text{C.}$ We have
>
> $\psi:\ D + F = B + C.$ (15)
>
> $\frac{d\psi}{\text{dx}}:\ \frac{i}{h}D - \frac{i}{h}E = \frac{}{h}B - \frac{}{h}\text{C.}$
> (16)
>
> If we multiply equation (15) by $i$ and solve simultaneously with
> equation (16) we get
>
> $F = \frac{(\  - \ i)B\  - \ (\  + \ i)C}{- 2i}$ (17)
>
> and
>
> $D = \frac{(\  + \ i)B\  + \ (i - \ )C}{2i}$ (18)
>
> As we found before, the value of $B$ is negligible for certain
> parameters so let us set $B = 0.$
>
> Now we have the two equations
>
> $D = \frac{(1 + i)}{2}C$ (19)
>
> and
>
> $F = \frac{(1 - i}{2}\text{C.}$ (20)
>
> Now we have $D$ and $F$ in terms of $C,$ and $C$ in terms of
> $\text{A.}$ Our general aim is to find the transmission coefficient
> i.e the probability of tunneling. We know $A$ is the coefficient of
> the wave equation of the outgoing wave because it has a positive power
> and is therefore moving from left to right. Further, $D$ is the
> coefficient for the incoming wave, so we can see that these are the
> two coefficients that are important to us. So let us now write $D$ in
> terms of $\text{A.}$ Substituting the value from equation (14) into
> equation (19) and writing $\kappa$ and $k$ in their full forms gives
>
> $D = \frac{(1 + i)}{2}\frac{(( - i)}{2}Ae^{\frac{}{\hslash}( + i)L}.$
> (21)
>
> Simplifying and rearranging to get $D$ and $A$ on the same side we
> have
>
> $\frac{D}{A} = \frac{1}{2}(1 + i)\frac{- i}{2}e^{\frac{}{\hslash}( + i)L}.$
> (22)
>
> In section three we discussed that the probability density could be
> found by finding the square of the magnitude of the wavefunction in
> the last region. For this problem we want to find the transmission
> coefficient, the ratio of the rate of outgoing particles to incoming
> particles. As a ratio, this is equal to
> $\frac{\left| A \right|^{2}}{\left| D \right|^{2}}.$ Starting from
> equation (22) we get
>
> $\frac{\left| D \right|^{2}}{\left| A \right|^{2}} = \frac{1}{4}(1 + \frac{V_{0} - E}{E})(\frac{V_{0} - E + E}{4(V_{0} - E)})e^{2}$
> (23)
>
> which simplifies to
>
> $\frac{\left| D \right|^{2}}{\left| A \right|^{2}} = \frac{V_{0}}{4E} \cdot \frac{V_{0}}{4(V_{0} - E)}e^{2L}.$
> (24)
>
> So
>
> $T =$$\frac{\left| A \right|^{2}}{\left| D \right|^{2}} = {\frac{16E(V_{0} - E)}{{V_{0}^{}}^{2}}e^{- 2L}}^{}.$
> (25)
>
> This is the probability of tunneling! We should be able to confirm two
> important pieces of information from equation (25). Firstly, we should
> see that when the length of the boundary $L$ is large and when
> $V_{0} - E$ is large, tunneling becomes less likely. Due to the
> negative power in the exponential factor, we can confirm that this is
> the case. Secondly, tunneling is certain when there is no potential
> barrier, so equation (25) should satisfy the condition that when
> $V_{0} = 0,\ T = 1.$ Since we have ${V_{0}^{}}^{2}$ in the
> denominator, this relationship will not be satisfied in our equation.
> This seems unusual but looking back at our initial wave functions, we
> assumed $V_{0} > E$ from the beginning. The solution depends on $$
> being real, but when we have $V_{0} = 0$ instead of $V_{0} > E$, this
> condition breaks and the calculation is therefore invalid for that
> value.
>
> Generally, this method can be used for most 1-D tunneling problems,
> provided we know the same pieces of information. Once one finds and
> substitutes the specific values for the particle being calculated for
> (mass and energy) as well as the potential of the system, a
> probability value can be found. However, this paper shows the
> base-level understanding of quantum tunneling and solves the barrier
> problem in the simplest, one-dimensional case. For applications of
> quantum tunneling to two-dimensional systems or to an atomic nucleus,
> a three-dimensional system, more advanced methods are required to
> predict the outcomes. Furthermore, we had assumed a ‘square’ potential
> for simplicity, but in actuality a potential barrier is not typically
> flat, and would need more intricate calculations. Qualitatively
> though, these systems behave in a similar way.
>
> Given more time, some further explorable topics relating to the
> applications of quantum tunneling could include its role in flash
> memory where particles tunnel preferentially when voltage is applied.
> Specifically, the MOSFET devices used in this incorporate tunneling
> particles in their design which allows for “considerable power
> savings” \[8\]. Quantum tunneling also explains radioactive decay,
> where particles tunnel despite the attractive nuclear force they are
> seemingly bound within.

**References**

\[1\] Oxford Languages Dictionary. *Potential Barrier*.
https://www.oed.com/.

\[2\] David Morin. *Waves*.
https://scholar.harvard.edu/david-morin/waves.

> \[3\] UNSW. *The Wave Equation and Wave Speed*.
> https://www.animations.physics.unsw.edu.au/jw/wave\_equation\_speed.htm\#equation
>
> \[4\] Physics Classroom. *Boundary Behaviour.*
> https://www.physicsclassroom.com/class/waves/Lesson-3/Boundary-Behavior
>
> \[5\] Linus Pauling. *Introduction to Quantum Mechanics with
> Applications to Chemistry.* Dover Publications, 1937/1985.
>
> \[6\] The Editors of Encyclopaedia Britannica. *Wave Function.
> https://www.britannica.com/science/wave-function*

\[7\] David Bohm. *Quantum Theory.* Dover Publications, 1951/1989.

> \[8\] Tech Briefs. *Quantum Tunneling Produces Record Transistor
> Performance.* January 2012.
> https://www.techbriefs.com/component/content/article/tb/insiders/et/stories/12755
