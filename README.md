# Complex numbers background

<p>
  Complex numbers are a necessary part of math which allows to give a solution to equations of the form:
  
  $x = \sqrt{- n} = in = \Im(n)$

  where $n > 0 \in R$.<br>
  Since this calculation doesn't follow $R$ field rules, another field is necessary to operate on these numbers, and guess what it's the complex field $C$. Now to avoid writing a book about fields math concepts: a field is a set of numbers, where an identity element exists, where every element (number) of the field has an inverse, and where two operations exist $(+, \times)$ and have some properties. We don't care about every single property of a field, what I want to say now is that the basic operations in $C$ behave differently compared to $R$. The interesting fact is that the equation above alone builds an entire field around itself.<br>
  Now before proceeding, I want to clarify one thing: the complex field is often associated to the $3rd$ dimension of the cartesian graph. There exist some tools [ https://hemisemidemipresent.github.io/complex3/ ] which help figuring out the three-dimensionality built by the complex field, since it often coexist with the two-dimensional cartesian graph $/R$ field in many functions/equations. Indeed the complex field "plane" share the $x-axis$ with the cartesian graph $/R$. But note that this doesn't necessarily mean that we are talking about dimensions. As humans we are dependent on visualize things graphically, but math is nothing but logic relations about quantities. If you think about the $C$ field as "another dimension" you are probably not right. Indeed $C$ **extends** $R$, an allows to operate on complex numbers, nothing more, nothing less.

  
</p>

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
