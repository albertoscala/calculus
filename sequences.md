# Sequences

## Table of Contents

- [Sequences](#sequences)
  - [Table of Contents](#table-of-contents)
  - [Definition](#definition)
  - [Notation](#notation)
  - [Graphical Meaning](#graphical-meaning)
  - [Convergence and Divergence](#convergence-and-divergence)

## Definition

First of all, let's define what a sequence is in an informal way.

A sequence is a list of numbers written in a specific order. It may or may not have an infinite number of terms.

Sequence terms are denoted as follow:

$$a_1 - first \space term$$

$$a_2 - second \space term$$

$$\vdots$$

$$a_n - n^{th} \space term$$

$$a_{n+1} - (n+1)^{st} \space term$$

$$\vdots$$

## Notation

A sequence can be represented in a few different ways. The most common ones are:

$$\lbrace a_1, a_2, \cdots, a_n, a_{n+1}, \cdots \rbrace \quad \lbrace a_n \rbrace \quad \lbrace a_n \rbrace_{n=1}^{\infty}$$

In the second and third notations, $a_n$ is usually given by a formula.

**Examples**

To understand better the concept of sequences, let's calculate the first 5 terms of the following sequences:

$$\lbrace \frac{n + 1}{n^2} \rbrace_{n=1}^{\infty} = \lbrace 2, \frac{3}{4}, \frac{4}{9}, \frac{5}{16}, \frac{6}{25}, \cdots \rbrace$$

$$\lbrace \frac{(-1)^{n + 1}}{2^n} \rbrace_{n=1}^{\infty} = \lbrace -1, \frac{1}{2}, -\frac{1}{4}, \frac{1}{8}, -\frac{1}{16}, \cdots \rbrace$$

## Graphical Meaning

In the previous examples we were treating the formulas as fuctions that can only have integer values.

$$f(n) = \frac{n + 1}{n^2} \qquad g(n) = \frac{(-1)^{n + 1}}{2^n}$$

This is an important concept in the study of sequences (and series). We are treating the sequence terms as an evaluation of a function that later on will allow us to do many things with sequences.

## Convergence and Divergence

Something that we might find very useful to know about a sequence is if it converges to a specific value or if it diverges to infinity.

**Theorem**

The sequence $\lbrace r^n \rbrace$ converges if $-1 < r \leq 1$ and diverges for all other values of $r$. Also,

$$\begin{equation}
    \lim_{n \to \infty} r^n = 
    \begin{cases}
      0, & \text{if}\ a=1 \\
      1, & \text{otherwise}
    \end{cases}
  \end{equation}$$