# Limits

## Table of Contents

- [Definition](#definition)
- [One-Sided Limits](#one-sided-limits)
- [Properties of Limits](#properties-of-limits)
  - [Sum property](#sum-property)
  - [Difference property](#difference-property)
  - [Product property](#product-property)
  - [Constant multiplication property](#constant-multiplication-property)
  - [Quotient property](#quotient-property)
- [Solving methods](#solving-methods)
  - [Direct substitution](#direct-substitution)

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

### Direct substitution

The limit of a function can be found by direct substitution. This method is used when the function is continuous at the point $a$.

It can be also applied to rational functions, only if the denominator is not zero.

For example, given the function $f(x) = \frac{x^{3}+4x^{2}-3}{x^{2}+5}$, the limit as $x$ approaches $-1$ is:

$$\lim_{x \to -1} \frac{x^{3}+4x^{2}-3}{x^{2}+5} = \frac{(-1)^{3}+4(-1)^{2}-3}{(-1)^{2}+5} = \frac{0}{6} = 0$$

This can be defined more formally as: If $P(x)$ and $Q(x)$ are polynomials and $Q(c) \neq 0$, then:

$$\lim_{x \to c} \frac{P(x)}{Q(x)} = \frac{P(c)}{Q(c)}$$
