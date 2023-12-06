# Vectors are objects that move through space

> Notes on David Dye's [course on Mathematics for Machine Learning: Linear Algebra](https://www.coursera.org/learn/linear-algebra-machine-learning)

## Dot Product

The Dot Product or the Scalar Product is a measure of how closely two vectors align, in terms of the directions they point.

Given vector $a$ and $b$, then the dot product is defined as:

$$
a \cdot b = \sum_{i=1}^{n} a_{i}b_{i}
$$

Dot Product is Commutative meaning that the order does not matter:

$$
a \cdot b = b \cdot a
$$

It is also distributive, so you can distribute it into parentheses:

$$
a \cdot (b + c) = a \cdot b + a \cdot c
$$

As well as associative:

$$
a \cdot (bc) = b (a \cdot c)
$$

## Magnitude or Mod
The size of a vector is called Magnitude or Mod and is notated and calculated as such:

$$
|a| = \sqrt{\sum^n_{i=1} a_i^2}
$$

Basically just the Pythagorean Theorem but can be multidimensional

## Scalar Projection

The Scalar Projection or Scalar Shadow shows the distance of a vector projected onto another vector. (?)

$$
\frac{a \cdot b}{|a|}
$$

## Vector Projection
If we wanted a direction attached to our scalar projection, then we just multiply it by $\frac{a}{|a|}$ to get:

$$
\frac{a \cdot b}{|a|^2}a
$$

## Basis Vectors

A Basis is a set of $n$ vectors that:

- (i) are not linear combinartion of each other (linearly independent)
- (ii) span the space
- The space is then n-dimensional

## Change basis vectors

If another set of vectors are orthographic (meaning they are at 90 degree angles away from each other) then you can change the point of reference for an already existing vector to the orthographic vectors.

$$
a_b = 
\begin{bmatrix}
\frac{a \cdot b_1}{|b_1|^2} \\
... \\
\frac{a \cdot b_n}{|b_n|^2}
\end{bmatrix}
$$