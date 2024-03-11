# Limits

## Table of Contents

- [Limits](#limits)
  - [Table of Contents](#table-of-contents)
  - [Definition](#definition)
  - [One-Sided Limits](#one-sided-limits)
  - [Properties of Limits](#properties-of-limits)
    - [Sum property](#sum-property)
    - [Difference property](#difference-property)
    - [Product property](#product-property)
    - [Constant multiplication property](#constant-multiplication-property)
    - [Quotient property](#quotient-property)
  - [Solving methods](#solving-methods)
    - [Substitution method](#substitution-method)
    - [Factoring method](#factoring-method)
    - [Conjugate method](#conjugate-method)
  - [Indeterminated Forms and L'Hôpital's Rule](#indeterminated-forms-and-lhôpitals-rule)
  - [Limits to Infinity](#limits-to-infinity)
  - [Well-Known Limits](#well-known-limits)

## Definition

Let $f(x)$ be a function. The limit is defined as the value that the function $f(x)$ approaches as $x$ approaches a certain value. The limit is denoted as $\lim_{x \to a} f(x)$.

In general the limits are equal to the value of the function, but this is only true if the function is continuous at the point $a$.

## One-Sided Limits

One-sided limits are differentiated as *right-hand limits* (when the limit approaches from the right) and *left-hand limits* (when the limit approaches from the left).

The right-hand limit is denoted as:

$$\lim_{x \to a^+} f(x) = L$$

While the left-hand limit is denoted as:

$$\lim_{x \to a^-} f(x) = L$$

## Properties of Limits

Given two functions $f(x)$ and $g(x)$, and their limits as $x$ approaches $a$, the following properties hold:

### Sum property

The limit of the sum of two functions is equal to the sum of their limits:

$$\lim_{x \to a} [f(x) + g(x)] = \lim_{x \to a} f(x) + \lim_{x \to a} g(x) = L + M$$

### Difference property

The limit of the difference of two functions is equal to the difference of their limits:

$$\lim_{x \to a} [f(x) - g(x)] = \lim_{x \to a} f(x) - \lim_{x \to a} g(x) = L - M$$

### Product property

The limit of the product of two functions is equal to the product of their limits:

$$\lim_{x \to a} [f(x) \cdot g(x)] = \lim_{x \to a} f(x) \cdot \lim_{x \to a} g(x) = L \cdot M$$

### Constant multiplication property

The limit of a function multiplied by a constant is equal to the constant multiplied by the limit of the function:

$$\lim_{x \to a} [k \cdot f(x)] = k \cdot \lim_{x \to a} f(x) = k \cdot L$$

### Quotient property

The limit of the quotient of two functions is equal to the quotient of their limits, provided that the limit of the denominator is not zero:

$$\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{\lim_{x \to a} f(x)}{\lim_{x \to a} g(x)} = \frac{L}{M}$$

## Solving methods

### Substitution method

The limit of a function can be found by substitution. This method is used when the function is continuous at the point $a$.

It can be also applied to rational functions, only if the denominator is not zero.

For example, given the function $f(x) = \frac{x^{3}+4x^{2}-3}{x^{2}+5}$, the limit as $x$ approaches $-1$ is:

$$\lim_{x \to -1} \frac{x^{3}+4x^{2}-3}{x^{2}+5} = \frac{(-1)^{3}+4(-1)^{2}-3}{(-1)^{2}+5} = \frac{0}{6} = 0$$

This can be defined more formally as: If $P(x)$ and $Q(x)$ are polynomials and $Q(c) \neq 0$, then:

$$\lim_{x \to c} \frac{P(x)}{Q(x)} = \frac{P(c)}{Q(c)}$$

### Factoring method

Consider the function $f(x) = \frac{x^2 - 9}{x+3}$ and the limit as $x$ approaches $-3$. We can sure use the substitution method, but we can also factor the numerator to simplify the function and then use the substitution method:

$$f(x) = \frac{x^2 - 9}{x+3} = \frac{(x+3)(x-3)}{x+3} = x-3$$

Then, the limit is:

$$\lim_{x \to -3} f(x) = \lim_{x \to -3} x-3 = -3-3 = -6$$

### Conjugate method

The conjugate method is used to simplify the function by multiplying the numerator and the denominator by the conjugate of the numerator. This method is used when the function is in the form $\frac{f(x)}{g(x)}$ and the limit as $x$ approaches $a$ is an undefined form.

The conjugate of a binomial $a+b$ is $a-b$. For example, the conjugate of $x+3$ is $x-3$.

**Example**

$$\lim_{x \to 5} \frac{\sqrt{x+11}-4}{x-5}$$

**Solution**

We start solving the limit by substitution:

$$\lim_{x \to 5} \frac{\sqrt{x+11}-4}{x-5} = \frac{\sqrt{x+11}-4}{x-5} = \frac{\sqrt{5+11}-4}{5-5} = \frac{0}{0}$$

The limit is in an undefined form, so we can try use the conjugate method to simplify the function and try again with the substitution method.

$$\lim_{x \to 5} \frac{\sqrt{x+11}-4}{x-5}  \cdot  \frac{\sqrt{x+11}+4}{\sqrt{x+11}+4}$$

$$\lim_{x \to 5} \frac{(x+11)-16}{(x-5)(\sqrt{x+11}+4)}$$

$$\lim_{x \to 5} \frac{x-5}{(x-5)(\sqrt{x+11}+4)}$$

We can simplify by the $x-5$ in the numerator and denominator and finally substitute

$$\lim_{x \to 5} \frac{1}{\sqrt{x+11}+4} = \frac{1}{\sqrt{5+11}+4} = \frac{1}{8}$$

## Indeterminated Forms and L'Hôpital's Rule

Previously, we have seen a limit that returned us the result of $\frac{0}{0}$. This is an example of an indeterminate form. As we have seen, we can solve these indeterminate forms by reformulating the problem, if it doesn't work, we can apply the Hôpital's rule.

L'Hôpital's rule states that:

If the limit $\lim_{x \to c} \frac{f(x)}{g(x)}$ results in one of the following indeterminate form:

$$\frac{0}{0},\quad \pm \frac{\infty}{\infty},\quad 0 \cdot \pm \infty,\quad \infty - \infty,\quad 0^0, 1^{\infty},\quad \infty^{0}$$

And if the $\lim_{x \to c} \frac{f'(x)}{g'(x)}$ exists with $g'(x) \neq 0$ then:

$$\lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}$$

**Examples**

Solve the following limit: $\lim_{x \to 0} \frac{e^x-1}{x}$

$$\lim_{x \to 0} \frac{e^x-1}{x} = \frac{1-1}{0} = \frac{0}{0}$$

Indeterminate form, we can apply L'Hôpital's rule:

$$\lim_{x \to 0} \frac{e^x}{1} = 1$$

Solve the following limit: $\lim_{x \to 0^+} x * \ln(x)$

$$\lim_{x \to 0^+} x * \ln(x) = 0 * \ln(0) = 0 * - \infty$$

Indeterminate form, we can apply L'Hôpital's rule, but before we have to rewrite the function as $\frac{f(x)}{g(x)}$:

$$x * \ln(x) = \frac{\ln(x)}{\frac{1}{x}}$$

Then, we can apply L'Hôpital's rule:

$$\lim_{x \to 0^+} \frac{\ln(x)}{\frac{1}{x}} = \lim_{x \to 0^+} \frac{\frac{1}{x}}{-\frac{1}{x^2}} = \lim_{x \to 0^+} -x = 0$$

## Limits to Infinity

While working with limits, sometimes we are also interested on what happens when a certain function $f(x)$ behaves when approaches infinity.

To work with limits to infinity, we can use the following properties:

1. Every function as a rate of growth. Generally speaking the hierarchy of growth is: 

$$x! > n^x > x^n > x \log{x} > x > \log{x} > n$$

2. If the degree of the numerator is less than the degree of the denominator, then the limit is equal to zero. The reason behind this is that the denominator grows faster than the numerator so we are dividing a smaller number by a larger number.

**Example**

Solve the following limit: $\lim_{x \to \infty} \frac{5x^3 - 2x^2 + 7x - 13}{12 - 2x + x^4}$

$$\lim_{x \to \infty} \frac{5x^3 - 2x^2 + 7x - 13}{12 - 2x + x^4} = \frac{x^3}{x^4} = \frac{1}{x} = \frac{1}{\infty} = 0$$

3. If the degree of the numerator is greater than the degree of the denominator, then the limit is equal to infinity. The reason behind this is that the numerator grows faster than the denominator so we are dividing a larger number by a smaller number.

**Example**

Solve the following limit: $\lim_{x \to \infty} \frac{x! - \log{x} + 1}{2^x +3x^5 - 5 \log{x}}$

$$\lim_{x \to \infty} \frac{x! - \log{x} + 1}{2^x +3x^5 - 5 \log{x}} = \lim_{x \to \infty} \frac{x!}{2^x} = \infty$$

4. If the degree of the numerator is equal to the degree of the denominator, then the limit is equal to the ratio of the leading coefficients.

**Example**

Solve the following limit: $\lim_{x \to \infty} \frac{3x^3 - 2x^2 + 7x - 13}{12x^3 - 2x^2 + x^4}$

$$\lim_{x \to \infty} \frac{3x^3 - 2x^2 + 7x - 13}{12x^3 - 2x^2 + x^4} = \lim_{x \to \infty} \frac{3x^3}{12x^3} = \frac{1}{4}$$

*Note*

The in all the function we just consider the leading terms ignoring the rest of the terms because the character of the function is determined by the strongest term.

## Well-Known Limits

We have seen how to solve limits using different methods, but there are some limits that are well-known and can be used to solve other more complex limits. These can be solve using L'Hôpital's rule but to speed up the process we can memorise them. Some of these well-known limits are:

$$\lim_{x \to 0} \frac{\sin{x}}{x} = \lim_{x \to 0} \frac{\tan{x}}{x} = 1 \qquad \lim_{x \to 0} \frac{\arcsin{x}}{x} = \lim_{x \to 0} \frac{\arctan{x}}{x} = 1$$

$$$$

$$\lim_{x \to 0} \frac{e^x - 1}{x} = 1$$

$$\lim_{x \to 0} \frac{a^x - 1}{x} = \ln{a}$$

$$\lim_{x \to 0} \frac{\ln{x + 1}}{x} = 1$$

$$\lim_{x \to 0} (1 + x)^{\frac{1}{x}} = \lim_{|x| \to \infty} (1 + \frac{1}{x})^x = e$$

$$\lim_{x \to 0} (1 + x)^{\frac{1}{x}} = e$$

$$\lim_{x \to 0} \frac{x - \sin{x}}{x^3} = \frac{1}{6}$$

$$\lim_{x \to 0} \frac{x - \ln{1 + x}}{x^2} = \frac{1}{2}$$

$$\lim_{x \to 0} \frac{e - (1 + x)^{\frac{1}{x}}}{x} = \frac{e}{2}$$