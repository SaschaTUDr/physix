---
title: Introduction
---

## Nature of science
The main goal of physics, as well as other natural sciences such as chemistry and biology, is to understand how nature works. Although this goal is way too ambitious for humans to ever fully reach, people are relentlessly moving towards it. Different paths were taken in this endeavour since ancient times, but by far the most efficient one, usually known as **scientific method**, became common since at least the 17th century.

Scientific method is an iterative ongoing process featuring certain elements such as **observations**, from which a **research question** can be formulated and a **hypothesis** can be proposed. The hypothesis is then rigorously tested in **experiments** by acquiring and consistently analysing data so that a valid conclusion can be formulated. This conclusion can lead to a new **theory** (can as well be an improvement of some older theory), which can then be tested again in the similar way.

The key benefit of the scientific method lies in that hypotheses must be **falsifiable** (i. e. in case the hypothesis is wrong, it should be possible to deduce that from the data) and experiments must be **reproducible** (i. e. other people can repeat them obtaining results that do not contradict original conclusions). Reproducibility of results (and overall quality of the work) can be asserted by publishing the investigation in peer-reviewed journals.

Note that science is a creative process, and, in some investigations, accents can be shifted from one element of the scientific method to another, some elements can be omitted while others, not mentioned above, can appear. You can read more about the scientific method in Refs. [@IBPhysicsGuide;@ScientificMethod].


## Quantities and units
Data is the key output of the experiment, which is obtained through measurement (possibly followed by some analysis), and a physical **quantity** is a parameter (such as length, mass, density, speed etc.) that can be measured. The result of the measurement of a quantity is the numerical value multiple of a **unit of measurement**. For example, you can say that the length of a table is $1{,}05\,\mathrm{m}$, where $\mathrm{m}$ (stands for ‘metre’) is a unit of length. Units can be chosen freely as long as they are associated with the same quantity, so, one can as well say that the table from the previous example is $41{,}3\,\mathrm{in}$ or $3{,}44\,\mathrm{ft}$ long.


## International system of units
You might have noticed that people from different localities might use different units of measurement. During the Middle Ages this probably was not too big an issue, but as communication – especially scientific – between people in different countries became more and more frequent, the need for the unification of units arised. There were several attempts at that before in 1961 the International System of Units (commonly known by the abbreviation **SI** stemming from its French name – _Système international d'unités_) was introduced and is now _the_ system of units to be used for communicating science throughout the world.

SI builds up on seven **base units**: second ($\mathrm{s}$) for time, metre ($\mathrm{m}$) for length, kilogram ($\mathrm{kg}$) for mass, ampere ($\mathrm{A}$) for electric current, kelvin ($\mathrm{K}$) for temperature, mole ($\mathrm{mol}$) for amount of substance and candela ($\mathrm{cd}$) for luminous intensity.[^fn:SI]

Units for all other quantities can be derived using the definitions (hence the name **derived units**). For example, if speed $v$ is the covered distance $L$ divided by time $t$, then its SI unit is
:::{math}
:enumerated: false
  [v]=\frac{[L]}{[t]}=\mathrm{\frac{m}{s}},
:::
where the square brackets around the symbol of a quantity are used to extract its unit only. As another example, consider density, which is defined as mass $m$ per volume $V$. The volume itself (of a cuboid, without the loss of generality) is a product of three lengths, say, $a$, $b$ and $c$. Hence, SI unit of density is
:::{math}
:enumerated: false
  [\varrho]
  =\left[\frac{m}{V}\right]
  =\frac{[m]}{[abc]}
  =\mathrm{\frac{kg}{m\cdot m\cdot m}}
  =\mathrm{\frac{kg}{m^3}}.
:::

SI unit for angles is **radian**, which is a derived unit. Recall that by definition, $1\,\mathrm{rad}$ is the angle that subtends an arc of the circumference the length of which is equal to the radius. Algebraically, an angle $\varphi$ expressed in radians is
:::{math}
:enumerated: false
  \varphi=\frac{\ell}{R}
  \quad\leadsto\quad
  [\varphi]=\frac{[\ell]}{[R]}
  =\mathrm{\frac{m}{m}}=1.
:::
Hence angle is a **dimensionless** quantity. Other dimensionless quantities, which you might have come across, are, e. g., percent ($\%$), bit ($\mathrm{b}$), decibel ($\mathrm{dB}$) etc.  

:::{note} Typographical conventions
Unfortunately, there are not so many letters and other symbols available to denote quantities, units, etc: the common available set is limited to Latin and Greek alphabets, a couple of characters from Hebrew and Cyrillic alphabets and several letter-like symbols. So it is far from uncommon to see the same letter denoting both the quantity and (usually inconsistent) unit. Although the context is usually enough to distinguish the two, in order to increase legibility, the symbols of quantities are _italicised_, whereas the symbols for units (also, numbers, text labels etc.) are not.

For example, both mass and metre use ‘m’ for a symbol, but the mass is typeset as $m$, whereas the metre is typeset as $\mathrm{m}$. This approach does not apply to handwritten text, as it is rather hard to change the scripts when writing, so the context will be the only help in discriminating between the two cases. 
:::

## Multiples of SI units
People usually do not like using too big or too small numbers, but sometimes the quantities will have either huge or tiny values if expressed in SI units. One of the ways to compensate for that is to add a prefix to the unit (see @tab:SI). Note that you cannot add more than one prefix to a unit. 

:::{table} Multiples of SI units
:label: tab:SI
  | Factor    | Name    | Symbol         | Factor     | Name    | Symbol         |
  | --------- | ------- | -------------- | ---------- | ------- | -------------- |
  | $10^1$    | deca-   | $\mathrm{da}$  | $10^{-1}$  | deci-   | $\mathrm{d}$   |
  | $10^2$    | hecto-  | $\mathrm{h}$   | $10^{-2}$  | centi-  | $\mathrm{c}$   |
  | $10^3$    | kilo-   | $\mathrm{k}$   | $10^{-3}$  | milli-  | $\mathrm{m}$   |
  | $10^6$    | mega-   | $\mathrm{M}$   | $10^{-6}$  | micro-  | µ           |
  | $10^9$    | giga-   | $\mathrm{G}$   | $10^{-9}$  | nano-   | $\mathrm{n}$   |
  | $10^{12}$ | tera-   | $\mathrm{T}$   | $10^{-12}$ | pico-   | $\mathrm{p}$   |
  | $10^{15}$ | peta-   | $\mathrm{P}$   | $10^{-15}$ | femto-  | $\mathrm{f}$   |
  | $10^{18}$ | exa-    | $\mathrm{E}$   | $10^{-18}$ | atto-   | $\mathrm{a}$   |
  | $10^{21}$ | zetta-  | $\mathrm{Z}$   | $10^{-21}$ | zepto-  | $\mathrm{z}$   |
  | $10^{24}$ | yotta-  | $\mathrm{Y}$   | $10^{-24}$ | yocto-  | $\mathrm{y}$   |
  | $10^{27}$ | ronna-  | $\mathrm{R}$   | $10^{-27}$ | ronto-  | $\mathrm{r}$   |
  | $10^{30}$ | quetta- | $\mathrm{Q}$   | $10^{-30}$ | quecto- | $\mathrm{q}$   |
:::


## Common non-SI units
Due to historical reasons or simply for convenience in some fields, certain non-SI units are commonly used. The ones you will see this year are:

- minute ($1\,\mathrm{min}=60\,\mathrm{s}$);
- hour ($1\,\mathrm{h}=3600\,\mathrm{s}$);
- day ($1\,\mathrm{d}=86400\,\mathrm{s}$);
- year ($1\,\mathrm{a}=3{,}155\ldots\cdot10^7\,\mathrm{s}$);
- degree ($1^\circ=\frac{\pi}{180}\,\mathrm{rad}$);
- litre ($1\,\ell=10^{-3}\,\mathrm{m^3}$);
- astronomical unit ($1\,\mathrm{ua}=1{,}496\ldots\cdot10^{11}\,\mathrm{m}$);
- bar ($1\,\mathrm{bar}=10^5\,\mathrm{Pa}$);
- torr or mmHg ($1\,\mathrm{Torr}=133{,}3\ldots\,\mathrm{Pa}$).


## Significant figures
Any measurement is neither absolutely accurate, nor absolutely precise. That means that the result of the measurement should better be stated as an interval. For example, if you measure the length of the table to be $110{,}5\,\mathrm{cm}$, the result may be quoted as $\ell\in[110{,}4;110{,}6]\,\mathrm{cm}$, taking into account the uncertainty of the instrument (in this case, most probably a tape measure). Another, shorter way to quote the same result is like this: $\ell=(110{,}5\pm0{,}1)\,\mathrm{cm}$. Note the use of brackets and units.

If the measurement is repeated with a more precise instrument, the result may be slightly different, but the first three figures – $1$, $1$ and $0$ – will be the same, and the figure $5$ might change just a little bit. The figures of the measurement result that are determined precisely or with a small uncertainty are called _significant_. In our example, all four figures are significant.

Using intervals or the plus-minus notation is somewhat inconvenient when solving theoretical problems, so a simplified approach is used, when it is assumed that all the figures of the number except the zeros at the front are significant. So, e. g., the mass $m=74{,}2\,\mathrm{kg}$ is known to three significant figures (s. f.), the time $t=0{,}0013\,\mathrm{s}$ – to two s. f., the temperature $T=20{,}000\,\mathrm{^\circ C}$ – to five s. f. and the distance $d=3{,}0\cdot10^{-9}\,\mathrm{m}$ – to two s. f.

When **adding** or **subtracting** two quantities, the result will have as many **decimal places** as the quantity with the least number of decimal places, e. g.,
:::{math}
:enumerated: false
  2{,}0\,\mathrm{m}+0{,}52\,\mathrm{m}=2{,}5\,\mathrm{m},
:::
as the first quantity has one decimal place, but the seconond one – two. The result is thus rounded to one decimal place.

When **multiplying** or **dividing** quantities as well as raising a quantity to the **power** or taking a **root** thereof, the result will have as many **significant figures** as the quantity with the least number of significant figures, e. g.,
:::{math}
:enumerated: false
  \frac{6{,}0\,\mathrm{kg}\cdot0{,}0200\,\mathrm{m}}{(0{,}5\,\mathrm{s})^2}=0{,}03\,\mathrm{\frac{kg\,m}{s^2}},
:::
as the first quantity has two s. f., the second – three and the third – only one. The result is thus rounded to one s. f.

:::{warning}
  When performing calculations, apply rounding only to the final result, i. e. do not round the intermediate results. If you intend to use the result in further calculations, either save it in the calculator or keep at least one extra s. f.

  Use the regular equals-to sign ‘$=$’, not approximately-equals-to ‘$\approx$’ when writing the rounded results down. 
:::



[^fn:SI]: The official document that defines SI can be found [here](https://www.bipm.org/documents/20126/41483022/SI-Brochure-9-EN.pdf). You can also take a look at a more manageable [overview](https://www.bipm.org/en/measurement-units/si-base-units).