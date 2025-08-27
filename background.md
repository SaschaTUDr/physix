---
title: Mathematical background
---

Some say that mathematics is the language of physics, which is not untrue. You will save yourself quite a lot of effort while learning physics if you know – fluently – basics of elementary mathematics.

## Arithmetic
Addition, subtraction, multiplication and division of numbers should be easy:
:::{math}
:enumerated: false

\frac{(35+37)\cdot 1{,}2}{3{,}6}=24.
:::

Exponentiation, radicals and related properties should also be well-known:
:::{math}
:enumerated: false

2^{3}\cdot2^{-5}\cdot\sqrt{5^8}
=2^{-2}\cdot5^{8/2}=\frac{5^4}{2^2}=156{,}25
:::

Exponentiation has another inverse operation, _logarithm_, which comes in useful in the second year. Its basic idea can be illustrated with the following example:
:::{math}
:enumerated: false

2^8=256\quad\leftrightsquigarrow\quad\log_2256=8.
::: 

In physics, it is sometimes necessary to operate with very large or very small numbers. Using zeros for padding can be daunting and error prone, so scientific (standard) form of a number is used, e. g.
:::{math}
:enumerated: false
	\begin{aligned}
		25\,000\,000&=2{,}5\cdot10^7;\\
		0{,}000\,012&=1{,}2\cdot10^{-5}.
	\end{aligned}
:::

## Algebra
You should be (or make yourself) _very_ comfortable with rearranging algebraic expressions. For instance, expressing the height $h$ from Newton’s law of universal gravitation
:::{math}
:enumerated: false

F=G\frac{mM}{(R+h)^2}
\quad\leadsto\quad
h = \sqrt{\frac{GMm}{F}}-R
:::
should be done mentally and virtually automatically. For another example, you might need to express the distance $d_\mathrm{o}$ from the object to a thin lens of focal length $f$ given the distance $d_\mathrm{i}$ from the lens to the image:
:::{math}
:enumerated: false

\frac{1}{f}=\frac{1}{d_\mathrm{o}}+\frac{1}{d_\mathrm{i}}
\quad\leadsto\quad
d_\mathrm{o}=\frac{d_\mathrm{i}f}{d_\mathrm{i}-f}.
:::

Solving systems of equations is another skill you will use a lot. For that, you can use any method you know (substitution, addition, Gauß–Jordan elimination, Cramer rule, etc.). As an example, consider a problem, where you need to find the acceleration $a$ of a box on an inclined plane. Newton’s second law yields the following system of equations:
:::{math}
:enumerated: false

\left\{\begin{aligned}
	N-mg\cos\theta&=0\\
	mg\sin\theta-\mu N&=ma
\end{aligned}\right.
:::
from which you can obtain $a=g(\sin\theta-\mu\cos\theta)$ by expressing $N$ from the first equation and plugging it into the second one.

## Trigonometry
You are probably already familiar with three basic trigonometric functions (sine, cosine, tangent) as ratios of the sides of a right-angle triangle. This is the interpretation you will use most of the time. Sometimes, however, you will need to operate with trigonometric functions in a more abstract way, by using, e. g., reduction formulae, such as
:::{math}
:enumerated: false

\begin{aligned}
	\sin\left(\frac\pi2-\theta\right)&=\cos\theta, \\
	\sin\left(\pi-\theta\right)&=\sin\theta, \\
	\cos\left(\frac\pi2-\theta\right)&=\sin\theta, \\
	\cos\left(\pi-\theta\right)&=-\cos\theta,
\end{aligned}
:::
or functions of a double angle
:::{math}
:enumerated: false

\begin{aligned}
	\sin2\theta&=2\sin\theta\cos\theta,\\
	\cos2\theta&=\cos^2\theta-\sin^2\theta.
\end{aligned}
:::
You should also be familiar with both degrees and radians as units for a measure of an angle. Recall that one full turn is $360^\circ$ or $2\pi\,\mathrm{rad}$.

## Geometry
Some physics problems require using geometry. Most of the time this will have to do with calculating areas of regular shapes (rectangles, triangles, trapezia, circles, etc.):
:::{math}
:enumerated: false

\begin{aligned}
	S_\mathrm{rect}&=ab, \\
	S_\mathrm{tri}&=\frac{ah_a}2=\frac{ab\sin\gamma}2, \\
	S_\mathrm{trap}&=\frac{a+b}{2}\cdot h,\\
	S_\mathrm{circ}&=\pi R^2=\frac{\pi D^2}{4},
\end{aligned}
:::
and volumes of regular bodies (cuboids, cylinders, spheres):
:::{math}
:enumerated: false

\begin{aligned}
	V_\mathrm{cub}&=abc, \\
	V_\mathrm{cyl}&=S_\mathrm{base}h, \\
	V_\mathrm{sph}&=\frac43\pi R^3=\frac16\pi D^3.
\end{aligned}
:::
Occasionally, you will find the law of sines and the law of cosines useful:
:::{math}
:enumerated: false

\begin{gathered}
	\frac{a}{\sin\alpha}=\frac{b}{\sin\beta}=\frac{c}{\sin\gamma}=2R,\\
	c^2=a^2+b^2-2ab\cos\gamma.
\end{gathered}
::: 

## Vectors
Some physical quantities (e. g. velocity, force, displacement etc.) hold information not only about the magnitude, but also about the direction. Mathematically, these quantities are represented with vectors. You will work with vectors rather frequently, so you will need to know how they are added, subtracted, multiplied by a number and resolved along (or projected onto) given axes (see [](#fig:vectors)).

:::{figure} figures/vectors.svg
:label: fig:vectors

Operations on vectors: addition, subtraction, multiplication by a number, resolution along given axes.
:::

You should also know, how addition, subtraction and multiplication by a number can be performed on vectors when they are expressed in components (coordinates, projections):
:::{math}
:enumerated: false

\begin{gathered}
	\bm{F}_1=\left(F_{1x},F_{1y}\right),\quad
	\bm{F}_2=\left(F_{2x},F_{2y}\right), \\
	\bm{F}_1\pm\bm{F}_2=\left(F_{1x}\pm F_{2x},F_{1y}\pm F_{2y}\right), \\
	\lambda\bm{F}_1=\left(\lambda F_{1x},\lambda F_{1y}\right).
\end{gathered}
:::
Components (coordinates, projections) of a vector are related to its magnitude and the angle it forms with the $x$ axis in a straightforward way. Denoting the magnitude of the vector $\bm{F}$ as $F=\|\bm{F}\|$ and the angle it forms with the $x$ axis as $\varphi{}$, we can use basic trigonometry and Pythagoras theorem to express
:::{math}
:enumerated: false

\begin{aligned}
	F_x&=F\cos\varphi, &
	F&=\sqrt{F_x^2+F_y^2},\\
	F_y&=F\sin\varphi, &
	\varphi&=\arctan\frac{F_y}{F_x}~~\left(\pm\pi\right),
\end{aligned}
:::
where in the last expression care needs to be taken as, on a full circle, there will always be two angles, which differ by $\pi{}$, with the same tangent.

Two vectors can be multiplied several ways. The scalar (dot) product between, say, vectors $\bm{F}$ and $\bm{s}$, is a scalar given by
:::{math}
:enumerated: false

\bm{F}\cdot\bm{s}
=Fs\cos\widehat{(\bm{F},\bm{s})}
=F_xs_x+F_ys_y,
:::
where $\widehat{(\bm{F},\bm{s})}$ is the angle between the vectors.

Slightly more complicated is the vector (cross) product, which you will come across in the second year. A vector product between, say, vectors $\bm{r}$ and $\bm{F}$ is a vector,[^fn:pseudovector] which is perpendicular to both $\bm{r}$ and $\bm{F}$ (the actual direction is given by the [right hand rule](wiki:Cross_product)) and the magnitude of which is
:::{math}
:enumerated: false

\lVert\bm{r}\times\bm{F}\rVert
=rF\sin\widehat{(\bm{r},\bm{F})}.
:::

(sec:derivatives)=
## Derivatives
You are not required to know how to do calculus properly during the first year, but the ideas behind derivatives and integrals will appear from time to time. Here is a brief introduction you might find useful.

Suppose you are driving a car, but your speedometer is broken. If you want to estimate your instantenous speed, you can measure the distance $\Delta L$ covered in some short time interval $\Delta t$. Using these, you can reasonably estimate your speed to be
:::{math}
:enumerated: false
	v_\mathrm{avg}=\frac{\Delta L}{\Delta t}.
:::
By taking smaller time intervals, you can get better estimates for the instanteneous speed, and in the limit when $\Delta t$ becomes infinitesimal, the correct result is obtained:
:::{math}
:enumerated: false
	v=\lim_{\Delta t\to0}\frac{\Delta L}{\Delta t}=\frac{\mathrm{d}L}{\mathrm{d}t}.
:::
In order to distinguish infinitesimal changes from finite ones, $\Delta{}$ is replaced by $\mathrm{d}$ and the limit symbol can be dropped.

::::{note} Derivative
A ratio of the infinitesimal change of the function over the infinitesimal change of its argument is called a **derivative**. Formally,
:::{math}
:enumerated: false

\frac{\mathrm{d}f(x)}{\mathrm{d}x}
\stackrel{\mathrm{def}}{=}
\lim_{\Delta x\to0}\frac{f(x+\Delta x)-f(x)}{\Delta x}.
:::
The derivative shows how ‘fast’ the function is changing.
::::

Derivatives have a clear graphical interpretation. Consider the previous example of estimating the speed of the car. If we plot the distance $L$ as a function of time $t$, then higher speed would mean steeper graph (you go further in the same time when moving with higher speed). In order to determine the speed graphically, you construct a _tangent_ to the $L(t)$ graph at the given point. The slope of this line will be the speed. More generally, the slope of the tangent to $L(t)$ graph is equal to the derivative of $L$ with respect to $t$ (see [](#fig:derivative)).

:::{figure} figures/derivative.svg
:label: fig:derivative
The slope of the tangent to the graph of the function is equal to the derivative of this function.
:::

## Integrals
Now consider a problem opposite to the one described in the previous section. You are driving a car and the speedometer is working alright, but the odometer is not. Say, you want to estimate the distance you have travelled in some time, but the problem is that your speed keeps changing all the time. What you can do is to split the total driving time into lots of small time intervals $\Delta t$ and to assume that during each such interval the speed does not change significantly and is approximately equal to the average speed $v_i$ on this interval. The distance covered in that time interval is then $\Delta L=\bar{v}_i\,\Delta t$, and the total distance is just the sum of all these little $\Delta L$’s, i. e.
:::{math}
:enumerated: false

L=\sum_i\bar{v}_i\Delta t.
:::
Along the lines of the previous section, the smaller $\Delta t$’s we take, the better our estimate for the total distance will be. In the limit of infinitesimal time intervals, the correct result is obtained:
:::{math}
:enumerated: false

L=\lim_{\Delta t\to0}\sum_i\bar{v}_i\Delta t=\int_{t_0}^{T}v\,\mathrm{d}t,
:::
where $t_0$ and $T$ are the initial and the final time moments and the sum of infinitesimals is denoted with a ‘long s’ (_ſ_ for ‘sum’).

::::{note} Integral
A sum of products of a function and an infinitesimal change of the argument over a given interval of the arguments is called a (definite) **integral**. Formally,
:::{math}
:enumerated: false

\int_{x_1}^{x_2}f(x)\,\mathrm{d}x
\stackrel{\mathrm{def}}{=}
\lim_{\Delta t\to0}\sum_i{f}(x_i)\Delta x.
:::
::::
Definite integrals have a clear graphical interpretation. Consider the previous example. If we plot the speed $v$ as a function of time $t$, then the distance $\Delta L=\bar{v}_i\Delta t$ covered by the car in a short period of time can be interpreted as the area of a rectangle with sides of $v$ and $\Delta t$ as shown in [](#fig:integral). Making $\Delta t$ very small and adding up all such infinitesimal areas will yield the total distance covered. More generally, the area between the graph of $v(t)$ and the time axis for a given interval of time is equal to the integral of $v(t)$ on this interval.

:::{figure} figures/integral.svg
:label: fig:integral
The area between the graph of the function and the abscissa axis is equal to the integral of this function on a given interval of arguments.
:::

Extra care is needed here: the ‘area’ is actually signed. It is negative if the graph is below the abscissa axis or if the final value of argument is less than the initial one.

[^fn:pseudovector]: Pseudovector, to be precise, as its direction changes to the opposite upon reflection in the plane parallel to it