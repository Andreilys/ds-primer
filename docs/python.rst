.. python:

========
Python
========

.. contents:: :local:


.. _introduction:

Introduction
============

You need to know some basic calculus in order to understand how functions change over time (derivatives), and to calculate the total amount of a quantity that accumulates over a time period (integrals). The language of calculus will allow you to speak precisely about the properties of functions and better understand their behaviour.

Normally taking a calculus course involves doing lots of tedious calculations by hand, but having the power of computers on your side can make the process much more fun. This section describes the key ideas of calculus which you'll need to know to understand machine learning concepts.


.. loops:

Loops
===========


.. rubric:: Code


Let's write code to calculate the derivative of any function :math:`f(x)`. We test our function works as expected on the input :math:`f(x)=x^2` producing a value close to the actual derivative :math:`2x`.

::

  def get_derivative(func, x):
      """Compute the derivative of `func` at the location `x`."""
      h = 0.0001                          # step size
      return (func(x+h) - func(x)) / h    # rise-over-run

  def f(x): return x**2                   # some test function f(x)=x^2
  x = 3                                   # the location of interest
  computed = get_derivative(f, x)
  actual = 2*x

  computed, actual   # = 6.0001, 6        # pretty close if you ask me...


In general it's preferable to use the math to obtain exact derivative formulas, but keep in mind you can always compute derivatives numerically by computing the rise-over-run for a "small step" :math:`h`. 



.. rubric:: References

.. [1] https://en.wikipedia.org/wiki/Derivative
.. [2] https://www.khanacademy.org/math/multivariable-calculus/multivariable-derivatives/partial-derivative-and-gradient-articles/a/directional-derivative-introduction
.. [3] https://en.wikipedia.org/wiki/Partial_derivative
.. [4] https://en.wikipedia.org/wiki/Gradient
.. [5] https://betterexplained.com/articles/vector-calculus-understanding-the-gradient
.. [6] https://www.mathsisfun.com/calculus/derivatives-introduction.html
.. [7] http://tutorial.math.lamar.edu/Classes/CalcI/DefnOfDerivative.aspx
.. [8] https://www.khanacademy.org/math/calculus-home/taking-derivatives-calc/chain-rule-calc/v/chain-rule-introduction
.. [9] http://tutorial.math.lamar.edu/Classes/CalcI/ChainRule.aspx
.. [10] https://youtu.be/pHMzNW8Agq4?t=1m5s
.. [11] https://en.wikipedia.org/wiki/Dot_product
