---
title: Accelerated motion
label: sec:accelerated-motion
---

Consider again the train on the track (see [Uniform motion](#fig:train-on-track)). This time, rather than moving uniformly, the train is gaining velocity at a constant rate. Such a motion is called **uniformly accelerated**. If we denote the initial velocity of the train as $v_{0x}$, its velocity at time $t$ as $v_x$ and the rate of change of velocity – in other words, acceleration – as $a_x$, then
:::{math}
:label: eq:accelerated-v-t
	v_x(t)=v_{0x}+a_xt.
:::
Recall that the displacement is equal to the (signed) area under $v_x(t)$ graph. In the case of a uniformly accelerated motion, the $v_x(t)$ graph, as per @eq:accelerated-v-t, is a line with the slope $a_x$ passing through the point $(0;v_{0x})$ as shown in @fig:accelerated-motion-graph.

:::{figure} figures/accelerated-graph.svg
:label: fig:accelerated-motion-graph
Graph of velocity $v_x$ vs. time $t$ in a uniformly accelerated motion. The area between the graph and the time axis is the displacement $s_x$.
:::

The displacement of the train is thus equal to the area of the coloured trapezium
:::{math}
:label: eq:accelerated-s
	\begin{aligned}
		s_x&=\frac{v_{0x}+v_x}{2}\cdot t \\
		&=\frac{v_{0x}+(v_{0x}+a_xt)}{2}\cdot t \\
		&=v_{0x}t+\frac{a_xt^2}{2}.
	\end{aligned}
:::
Taking into account that by definition $s_x=x-x_0$, we finally can write that
:::{math}
:label: eq:accelerated-x-t
	x(t)=x_0+v_{0x}t+\frac{a_xt^2}{2}.
:::

::::{seealso} Displacement as an integral
:class: dropdown
A geometrical operation of finding the area between the graph and the abscissa axis has, as you might recall, an analytical counterpart: The value of this area is an integral of the function on the given interval. Hence, displacement performed by an object from time $t_1$ to time $t_2$ is
:::{math}
:enumerated: false
	s_x=\int_{t_1}^{t_2}v_x(t)\,\mathrm{d}t.
:::
In the case of a uniformly accelerated motion, setting $t_1=0$, $t_2=t$ and renaming the integration variable to $\tau$, we get that
:::{math}
:enumerated: false
	\begin{aligned}
		s_x&=\int_0^t v_x(\tau)\,\mathrm{d}\tau \\
		&=\int_0^t(v_{0x}+a_x\tau)\,\mathrm{d}\tau \\
		&=\int_0^t v_{0x}\,\mathrm{d}\tau+\int_0^t a_x\tau\,\mathrm{d}\tau \\
		&=v_{0x}t+a_x\frac{t^2}{2},
	\end{aligned}
:::
exactly the same result that was obtained previously. In this particular case integration does not help much, but if velocity dependence on time becomes complicated, analytical approach becomes more preferable.
::::

::::{note} Accelerated motion in different variables
A uniformly accelerated motion can be described using five quantities: displacement $s_x$, initial velocity $v_{0x}$, current velocity $v_x$, acceleration $a_x$ and time $t$. Note that any three of these quantities are _independent_, and the remaining two quantities can be uniquely determined from the given three. For example, if $v_{0x}$, $v_x$ and $t$ are known, then $a_x$ and $s_x$ can be expressed using @eq:accelerated-v-t and @eq:accelerated-s, respectively. 

A useful expression that you will frequently encounter is the one relating $s_x$, $a_x$, $v_x$ and $v_{0x}$ and lacking time. We start by expressing $s_x$ in terms of $v_x$, $v_{0x}$ and $t$ as per @eq:accelerated-s and then substituting $t$ from @eq:accelerated-v-t:
:::{math}
:label: eq:accelerated-s-v
	\begin{aligned}
		s_x&=\frac{v_x+v_{0x}}{2}\cdot t \\
		&=\frac{v_x+v_{0x}}{2}\cdot\frac{v_x-v_{0x}}{a_x} \\
		&=\frac{v_x^2-v_{0x}^2}{2a_x}.
	\end{aligned}
:::
::::

::::{exercise}
:label: ex:equation-accelerated-motion
A particle is moving along the $x$ axis so that its equation of motion, in SI units, is
:::{math}
:enumerated: false
	x(t)=1{,}0t^2-2{,}0t+3{,}0.
:::

1. What is the (i) initial coordinate, (ii) initial velocity and (iii) acceleration of the particle?
1. Write down the equation of particle's velocity $v_x(t)$.
1. At what moment does the particle stop? 
1. Is the speed of the particle increasing or decreasing at (i) $t=0$, (ii) $t=2{,}0\,\mathrm{s}$?
::::
::::{solution} ex:equation-accelerated-motion
:class: dropdown

Consider the general form of the equation of uniformly accelerated motion @eq:accelerated-x-t. Here, the free term is the initial coordinate $x_0$, the quantity multiplied by time $t$ is the initial velocity $v_{0x}$ and the quantity multiplied by $t^2$ is the _half_ of acceleration $a_x$. In the equation from the exercise, the free term is $3{,}0$, the prefactor of $t$ is $-2{,}0$ and the prefactor of $t^2$ is $1{,}0$. Hence, restoring SI units for the quantities, we get that $x_0=3{,}0\,\mathrm{m}$, $v_{0x}=-2{,}0\,\mathrm{m\,s^{-1}}$ and $a_x=2\cdot1{,}0=2{,}0\,\mathrm{m\,s^{-2}}$.

The velocity of the particle, in SI units, is
:::{math}
:enumerated: false
	\begin{aligned}
		v_x(t)&=v_{0x}+a_xt \\
		&=-2{,}0+2{,}0t.
	\end{aligned}
:::

The particle stops when its velocity is equal to zero, so
:::{math}
:enumerated: false
	\begin{gathered}
		v_{0x}+a_xt^*=0, \\
		t^*=-\frac{v_{0x}}{a_x}=1{,}0\,\mathrm{s}.
	\end{gathered}
:::

The speed of the particle is increasing (i.&thinsp;e. the partcile is ‘accelerating’) when $v_x$ and $a_x$ have the same sign. If not, the speed of the particle is decreasing (i.&thinsp;e. the particle is ‘decelerating’). In the exercise, $a_x>0$ all the time. Initially, $v_x=v_0<0$, so the speed of the particle decreases, while at $t=2{,}0\,\mathrm{s}$, $v_x=-2{,}0+2{,}0\cdot2{,}0>0$, so the speed of the particle increases.
::::