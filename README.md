# Complex numbers background

<p>
  Complex numbers are a necessary part of math which allows to give a solution to equations of the form
  
  $x = \sqrt{- n} \notin R$<br>
  $->$<br>
  $x = \sqrt{- n} = i\sqrt{n} = Im(\sqrt{n}) \in C$

  where $n > 0 \in R$.
  
  Since this calculation doesn't follow $R$ field rules, another field is necessary to operate on these numbers, and guess what it's the complex field $C$. Now to avoid writing a book about fields math concepts: a field is a set of numbers, where an identity element exists, where every element (number) of the field has an inverse, and where two operations exist $(+, \times)$ and have some properties. We don't care about every single property of a field, what I want to say now is that the basic operations in $C$ behave differently compared to $R$. The interesting fact is that the equation above alone builds an entire field around itself.<br>
  Now before proceeding, I want to clarify one thing: the complex field is often associated to the $3rd$ dimension of the cartesian graph. There exist some tools [https://hemisemidemipresent.github.io/complex/] which help figuring out the three-dimensionality built by the complex field, since it often coexist with the two-dimensional cartesian graph $/R$ field in many functions/equations. Indeed the complex field "plane" share the $x-axis$ with the cartesian graph $/R$. But note that this doesn't necessarily mean that we are talking about dimensions. As humans we are dependent on visualize things graphically, but math is nothing but logic relations about quantities. If you think about the $C$ field as "another dimension" you are probably not right. Indeed $C$ **extends** $R$, and allows to operate on complex numbers, nothing more, nothing less. Math research permits to describe new logic behaviours about quantities which in turn permit to solve other problems. To conclude, don't stick too much on the dimensions, even though having a look at the above link could be useful.

![C](C.png)

</p>

## Representation and multiplication of numbers in $C$

<p>
  Since

  $n > 0, \sqrt{- n} = i\sqrt{n}$<br>
  $->$<br>
  $(\sqrt{- n})^{2} = - n = (i\sqrt{n})^{2} = i^{2}(\sqrt{n})^{2}$

  it must be that

  $i^{2} = i \cdot i = - 1$

  When we deal with the cartesian graph, every point mapped on it can be represented using this form:

  $(x_{?}, y_{?})$

  We can notice that this representation is the same as $x_{?} + y_{?}$, indeed this form is called "algebraic". Now since (as already mentioned) $C$ field shares $x-axis$ with $R$, infact $C$ is an **extension** of $R$ (as shown above into the Euler-Venn graph), we can represent complex numbers as sitting on an orthogonal to $R$ plane (see the link above and play around, this is why I told you that it could be useful to visualize it). This reasoning is to "justify" the presence of a "real" part in the $C$ field. To better understand this fact, the following are the 2D (Re, and Im) **and** 3D representation of $y = \sqrt{x}$ function

  ![sqrtRe](sqrtRe.png)

  which as you can see is not defined when $n < 0$ since $\sqrt{n} \notin R$ for $n$ negative, while

  ![sqrtIm](sqrtIm.png)

  is exactly the same function but it is defined in $C$, indeed $n < 0, \sqrt{n} = i\sqrt{n} \in C$.<br>
  Now let's see the 3D representation, always noting that these results are somehow biased from the obvious complexity of such 
  software and the forced $3rd-person$ POV.

  ![sqrt3D](sqrt3D.png)

  Now, since we know why the $x-axis$ is shared between $R$ and $C$, and we can represent any number in an "algebraic" form:

  $z = (x, y) = x + y$ with $z, x, y \in R$ 
  
  is the representation of any number on the $R-plane$ part of the cartesian graph, while
  
  $z = (x, Im(y)) = x + Im(y)$ with $z, Im(y) \in C, x, y \in R$ 
  
  is the representation of any number on the $C-plane$ part of the cartesian graph.

  Now we can further observe a couple of complex numbers graphical representation in a clearer representation of the $C$ plane.

  $z_1 = 1 + Im(1)$<br>
  $z_2 = - 3 - Im(2)$

  ![CP](./CP.png)

  Now we can finally see the multiplication.

  $z_{1} = (x_{1}, Im(y_{1})) = x_{1} + Im(y_{1}) = x_{1} + iy_{1}$<br>
  $z_{2} = (x_{2}, Im(y_{2})) = x_{2} + Im(y_{2}) = x_{2} + iy_{2}$
  
  $(x_{1}, Im(y_{1})) \cdot (x_{2}, Im(y_{2})) = (x_{1} + iy_{1})(x_{2} + iy_{2}) = x_{1}x_{2} + x_{1}iy_{2} + iy_{1}x_{2} + (- 1)y_{1}y_{2} = x_{1}x_{2} - y_{1}y_{2} + i(x_{1}y_{2} + y_{1}x_{2}) = (x_{1}x_{2} - y_{1}y_{2}, x_{1}y_{2} + y_{1}x_{2})$
 
</p>

## Tigonometric shape of complex numbers

<p>
  Some basic knowledge of trigonometry enables us to represent complex numbers in a quite intuitive form which only involves the length of $z$ segment, and the $\sin$ and $\cos$ functions, which in turn is the exact same of the "algebraic" form.

  If you don't remember radians values for angles I give you a quick remainder. The circumference of a circle of radius $r = 1$ is given by

  $C = 2 \pi r$

  (because $\pi = C / 2r$).

  This means that we can represent the round angle ($360°$) $\theta$ as $(r = 1)$

  $\theta = 2\pi$

  and every other angle follows, then if
  
  $\theta = 180°$<br>
  $->$<br>
  $\theta = \pi$

  $-----$

  $\theta = 90°$<br>
  $->$<br>
  $\displaystyle \theta = \frac{\pi}{2}$

  and so on. We can safely set $r = 1$ as angles are not affected by the length of the radius, indeed it's clear that radians are the true representation of angles.

  Now, back to our complex numbers, since

  $z = x + Im(y) = x + iy$
  
  we can define $z \in C$ as

  $z = \sqrt{x^{2} + y^{2}}\cos(\theta) + \sqrt{x^{2} + y^{2}}i\sin(\theta)$

  where $\theta$ is the angle in the middle of the $z$ segment and the $x-axis$, and $\sqrt{x^{2} + y^{2}}$ is basically the formula derived by the Pitagorean Theorem which calculates the hypothenuse of a triangle, which in our case is exactly the $z$ segment, and for which you can find an intuitive graphical proof at [https://it.wikipedia.org/wiki/Teorema_di_Pitagora] (just watch the images). Now, calling

  $|z| = \sqrt{x^{2} + y^{2}}$<br>
  $->$<br>
  $z = |z|\cos(\theta) + |z|i\sin(\theta)$<br>
  $->$<br>
  $z = |z|(\cos(\theta) + i\sin(\theta))$

  we basically derived our trigonometric form for any complex number $z$, for which you can find a graphical representation below.

  ![CP2](./CP2.png)

</p>

## From Newton $e$ constant discovery to



#### Ex. $x^{2} - 1 = 0$

<p>
  $x^{2} - 1 = 0$<br>
  $x^{2} = 1$<br>
  $x = 1$ or $x = - 1$

  This is not a complex solution, since we don't have $x = \sqrt{- 1}$ but $\sqrt{x^{2}} = \pm \sqrt{1}$, and $x^{2} - 1 = 0$ equals:

  $(x - 1)[x - (- 1)] = (x - 1)(x + 1) = 0$
</p>

#### Ex. $x^{3} - 1 = 0$

<p>
  Now, let's look at why complex numbers are so fascinating:

  $x^{3} - 1 = 0$<br>
  $(x - 1)(x^2 + x + 1) = 0$<br>

  Here we know that $1$ is a solution for sure, but look at the other solutions:

  $x^2 + x + 1 = 0$

  Applying [ https://github.com/xyzhyn/Quadratic-formula-derivation ], we find:

  $\displaystyle x_{1} = \frac{- 1 + \sqrt{1^{2} - 4 \cdot 1 \cdot 1}}{2} = \frac{- 1}{2} + \frac{\sqrt{- 3}}{2}$

  $\displaystyle x_{2} = \frac{- 1 - \sqrt{1^{2} - 4 \cdot 1 \cdot 1}}{2} = \frac{- 1}{2} - \frac{\sqrt{- 3}}{2}$

  Hence the only way to break down $x^{3} - 1 = 0$ is:

  $\displaystyle (x - 1)[x - (\frac{- 1}{2} + \frac{\sqrt{- 3}}{2})][x - (\frac{- 1}{2} - \frac{\sqrt{- 3}}{2})]$
</p>

#### Ex. $x^{4} - 1 = 0$

<p>
  $x^{4} - 1 = 0$<br>
  $(x - 1)(x^{3} + x^{2} + x + 1) = 0$<br>
  $(x - 1)[(x + 1)(x^{2} + 1)] = 0$<br>
  $(x - 1)(x + 1)(x^{2} + 1) = 0$<br>

  We have $4$ solutions:

  $x = 1$<br>
  $x = - 1$<br>
  $x = \sqrt{- 1}$<br>
  $x = - \sqrt{- 1}$

  indeed

  $x^{4} - 1 = (x - 1)(x + 1)(x - \sqrt{- 1})(x + \sqrt{- 1})$<br>

 #### Ex. $x^{5} - 1 = 0$

 <p>
   $x^{5} - 1 = 0$<br>
   $(x - 1)(x^{4} + x^{3} + x^{2} + x + 1)$<br>
   $(x - 1)(x - 1)(x + 1)(x - \sqrt{- 1})(x + \sqrt{- 1})$

   Here we can recon that it's not true that $x^{n} - 1 = 0$ has **always** $n$ solutions.
 </p>

  
</p>
