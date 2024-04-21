# Integrals 

## Table of Contents

- [Integrals](#integrals)
  - [Table of Contents](#table-of-contents)
  - [Definite Integral](#definite-integral)
    - [Area Problem](#area-problem)

## Definite Integral

### Area Problem

The definite integral is the second type of integral that we can calculate. Before talking about the Definite Integrals, firstly we are going to take a look at the **Area Problem**.

The **Area Problem** is to definite integrals what the tangent and rate of change problems are to derivatives.

Let's start understanding the problem with an example.
Let $f(x) = x^2 - 1$ in the interval $[0, 2]$. In other words we want to determine the area below the graph.

We can't calculate the exact area, but we can approximate it by dividing the interval into $n$ subintervals of equal width $\Delta x = \frac{b - a}{n}$.

Then in each interval we can draw a rectangle with height $f(x_i)$ and width $\Delta x$.

Note that by choosing the height as we did each of the rectangles will over estimate the area of the subinterval, since the height of the rectangle is determined by the right endpoint of the interval.

The sum of the areas of the rectangles will be the total area of the region below the curve.

We can do the opposite, by choosing the height of the rectangle as the left endpoint of the interval, and we will have an underestimation of the area.

There is also a third way to estimate the area, by choosing the height of the rectangle as the midpoint of the interval.

Now let's suppose we want a better approximation of the area. We can do this by increasing the number of subintervals (aka increasing the number of rectangles), and therefore the width of each subinterval will decrease.

Now let's move on to the general case. Let $f(x)$ be a continuous function on the interval $[a, b]$ and we will divide the interval into $n$ subintervals of equal width $\Delta x = \frac{b - a}{n}$.

Note the interesting fact that the width of the subintervals shouldn't necessarily be equal, but it definitely makes the calculations easier.

Note that the endpoints of the subintervals are,

$$
x_0 = a \\
x_1 = a + \Delta x \\
x_2 = a + 2\Delta x \\
\vdots \\
x_i = a + i\Delta x \\
\vdots \\
x_{n-1} = a + (n-1)\Delta x \\
x_n = a + n\Delta x
$$

Where the sum of all the subintervals is equal to the total interval, $a + n\Delta x = b$.

Next in each subinterval we can choose a point $x_i^*$, *note same as before they don't have to be all in the same part of the subinterval but having them all in the same place will help us in the calculations*.

The area of the curve is then approximately the sum of the areas of the rectangles, $f(x_i^*)\Delta x$.

$$ A \approx f(x_1^{\ast})\Delta x + f(x_2^{\ast})\Delta x + \cdots + f(x_n^{\ast})\Delta x $$

Using summation notation we can write the area as,

$$ A \approx \sum_{i=1}^{n} f(x_i^*)\Delta x $$

This summation is better known as the **Riemann Sum**.

To get a better approximation of the area we can increase the number of subintervals, and therefore the width of each subinterval will decrease, that will lead us to the next notation,

$$ A = \lim_{n \to \infty} \sum_{i=1}^{n} f(x_i^*)\Delta x $$

Before we move on to the definition of the definite integral, let's take a look at what happens when the curve is below the x-axis.

In this case, the area of the curve will be negative, and the area of the region will be the sum of the areas of the rectangles.

This might create a problem with more complex functions that are both above and below the x-axis, since we are interested in the area of the region, and we don't want to have negative values.