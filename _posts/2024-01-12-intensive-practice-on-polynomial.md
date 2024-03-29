---
layout: post
title: "Polynomial, Intensive Practice on"
date: 2024-01-12 00:12:00 -0700
tags: ip algebra
comments: "true"
inlinecomments: "true"
mathjax: "true"
permalink: "ip/polynomial"
---
  Polynomial theorems and problems from past papers.

  Difficulty: AMC10/12, AIME

<!--more-->
  - [Definitions](#definitions)
  - [Theorems](#theorems)
  - [Problems](#problems)

### Definitions
- Polynomial

  $p(x) = a_nx^n + a_{n-1}x^{n-1} + a_{n-2}x^{n-2} + \cdots \cdots + a_2x^2 + a_1x + a_0$

  $a_n, a_{n-1}, \dots, a_2, a_1, a_0$ are coefficients. Specifically, $a_n$ is leading coefficient.

- Degree of Polynomial

  The highest of the degrees of the polynomial's monomials (individual terms) with non-zero coefficients.
  - Special case – zero
  - Degree 0 – non-zero constant
  - Degree 1 – linear
  - Degree 2 – quadratic
  - Degree 3 – cubic
  - Degree 4 – quartic (or, if all terms have even degree, biquadratic)
  - Degree 5 – quintic
  - Degree 6 – sextic (or, less commonly, hexic)
  - Degree 7 – septic (or, less commonly, heptic)
  - Degree 8 – octic
  - Degree 9 – nonic
  - Degree 10 – decic

- Zeros of Polynomial

  The points where the polynomial equals zero on the whole (e.g. $p(x)=0$).

### Theorems
- The Division Algorithm

  If $p(x)$ and $d(x) \not\equiv 0$ are any two polynomials then there exist unique polynomials $q(x)$ and $r(x)$ such that $p(x)=d(x) \cdot q(x) + r(x)$ where the degree of $r(x)$ is strictly less than the degree of $d(x)$ when the degree of $d(x) \geq 1$ or else $r(x) \equiv 0$.

  Long Division
  - Cheatsheet: [mathbitsnotebook](https://mathbitsnotebook.com/Algebra2/Polynomials/POPolyDivide.html){:target="_blank"}

  Synthetic Division
  - Cheatsheet: [mathbitsnotebook](https://mathbitsnotebook.com/Algebra2/Polynomials/POPolySynDivide.html){:target="_blank"}
  - More examples and applications: [purplemath](https://www.purplemath.com/modules/synthdiv.htm){:target="_blank"}
  - Divisor is trinomial: [wolfram](https://mathworld.wolfram.com/SyntheticDivision.html){:target="_blank"}

- Remainder Theorem

  When any polynomial $p(x)$ is divided by $x-a$ the remainder is $p(a)$.

- Factor Theorem

  $x-a$ is a factor of the polynomial $p(x)$ if and only if $p(a)=0$.

- Maximum Number of Zeros Theorem

  A polynomial cannot have more real zeros than its degree.

- Fundamental Theorem of Algebra

  a) Every polynomial of degree $n \geq 1$ has at least one zero among the complex numbers.

  b) If $p(x)$ denotes a polynomial of degree $n$, then $p(x)$ has exactly $n$ roots, some of which may be either irrational numbers or complex numbers.

- Complex Conjugate Roots Theorem (Complex number roots appear in conjugate pairs)

  If $p(x)$ is any polynomial with real coefficients, and if $a+bi$ is a complex root of the equation $p(x)=0$, then another complex root is its conjugate $a-bi$

- Irrational Conjugate Roots Theorem  (Irrational real roots appear in conjugate pairs)

  Let $p(x)$ be any polynomial with rational real coefficients. If $a+b\sqrt{c}$ is a root of the equation $p(x)=0$ where $\sqrt{c}$ is irrational and $a$ and $b$ are rational, then another root is $a-b\sqrt{c}$ has rational coefficients.)

- Odd Degree Real Root Theorem

  If $p(x)$ has real coefficients and has a degree that is odd then it has at least one real root.

- Intermediate Value Theorem

  If $p(x)$ is any polynomial with real coefficients, and if $p(a)>0$ and $p(b)<0$ then there is at least one real number $c$ between $a$ and $b$ such that $p(c)=0$

- [Vieta’s Formulas and the Identity Theorem](https://sites.math.washington.edu/~mathcircle/circle/2012-13/hw_2013_winter/VietasFormulas.pdf){:target="_blank"}

- [More Polynomial Theorems](https://monks.scranton.edu/files/courses/ProblemSolving/POLYTHEOREMS.pdf){:target="_blank"}

### Problems
- [$\star\star\star$] Given that the polynomial $x^2 - x - 1$ divides $ax^5 + bx^4 + 1$ without a remainder. Find the real numbers $a$ and $b$.
  <details>
    <summary>Answer</summary>
    a=3 and b=-5
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>The root of $x^2 - x - 1$ is also the root of $ax^5 + bx^4 + 1$.</li>
      <li>Vieta's Formula for Quadratic Equation.</li>
    </ul>
  </details>
   <br />

- [$\star$] If polynomial $x^2 - x + 1$ is a factor of polynomial $x^3 + x^2 + ax + b$ (where $a$ and $b$ are constants), what's the value of $a + b$?
  <details>
    <summary>Answer</summary>
    1
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>Polynomial Synthetic Division</li>
    </ul>
  </details>
   <br />

- [$\star\star\star$] Find the value of $f(2016)$ given that $f(x)$ is a polynomial of degree $2014$ such that $f(k) = \frac{1}{k}$ for every integer $k$ from $1$ to $2015$.
  <details>
    <summary>Answer</summary>
    1/1008
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>Polynomial Factor Theorem</li>
    </ul>
  </details>
   <br />

- [$\star$] Given distinct real numbers $a$, $b$, $c$, what's the simplified form of the algebraic expression $f(x) = \frac{a^2(x - b)(x - c)}{(a - b)(a - c)} + \frac{b^2(x - c)(x - a)}{(b - c)(b - a)} + \frac{c^2(x - a)(x - b)}{(c - a)(c - b)}$.
  <details>
    <summary>Answer</summary>
    f(x)=x<sup>2</sup>
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>Identity Theorem for Polynomials</li>
    </ul>
  </details>
   <br />

- [$\star$] Given that $p(x) = ax^3 + bx^2 + cx + d$ is a cubic polynomial satisfying $p(\frac{1}{2}) + p(-\frac{1}{2}) = 1000 \cdot p(0)$, and $x_1$, $x_2$, $x_3$ are the $3$ roots of $p(x) = 0$, What's the value of $\frac{1}{x_1x_2} + \frac{1}{x_2x_3} + \frac{1}{x_1x_3}$
  <details>
    <summary>Answer</summary>
    1996
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>Vieta's Formula.</li>
    </ul>
  </details>
   <br />

- [$\star\star$] Given the polynomial with integer coefficients $f(x) = x^5 + a_1x^4 + a_2x^3 + a_3x^2 + a_4x + a_5$, if $f(\sqrt{3} + \sqrt{2}) = 0$ and $f(1) + f(3) = 0$, what's the value of $f(−1)$.
  <details>
    <summary>Answer</summary>
    24
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>Polynomial Factor Theorem</li>
    </ul>
  </details>
   <br />

- [$\star$] If polynomial $f(x) = x^{12} − x^6 + 1$ is divided by $x^2 + 1$, yielding a quotient $q(x)$ and a remainder $r(x) = ax + b$, where $a$ and $b$ are real numbers, then what is the value of $b$?
  <details>
    <summary>Answer</summary>
    3
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>Polynomial Synthetic Division</li>
    </ul>
  </details>
   <br />

- [$\star\star$] If two of the roots of the quartic polynomial $x^4 − 18x^3 + kx^2 + 200x − 1984$ have product $−32$, what is the real number $k$?
  <details>
    <summary>Answer</summary>
    86
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>Vieta's Formula for Quadratic Equation.</li>
    </ul>
  </details>
   <br />

- [$\star\star$] If the quartic polynomial with integer coefficients $f(x)$ satisfies $f(1+\sqrt[3]{3}) = 1+\sqrt[3]{3}, f(1+\sqrt{3}) = 7+\sqrt{3}$, what is $f(x)$.
  <details>
    <summary>Answer</summary>
    f(x) = x<sup>4</sup> − 3x<sup>3</sup> + 3x<sup>2</sup> − 3x.
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>$f(a)=b$ means $a$ is the root of $f(x)-b=0$</li>
      <li>Polynomial Factor Theorem</li>
    </ul>
  </details>
   <br />

- [$\star$] If $x + y - 2$ is a factor of the polynomial $x^2 + axy + by^2 - 5x + y + 6$ with respect to $x$ and $y$, then what's the value of $a - b$?
  <details>
    <summary>Answer</summary>
    1
  </details>
   <br />

- [$\star\star$] What's the sum of all possible values of the integer $n$ such that the polynomial $f(x) = 3x^3 - nx - n - 2$ can be expressed as the product of two non-constant integer coefficient polynomials.
  <details>
    <summary>Answer</summary>
    192
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>$3x^3 - nx - n - 2 = (3x^2 + ax + b)(x − c)$</li>
      <li>$c = 0, −2, 4, −6$; $b = 2, −14, 10, 22$; $n = −2, 26, 38, 130$</li>
    </ul>
  </details>
   <br />

- [$\star\star$] If $p(x)$ is a quintic polynomial such that $x = 0$ is a triple root of $p(x) + 1 = 0$ and $x = 1$ is a triple root of $p(x) - 1 = 0$, what is $p(x)$ in expanded form?
  <details>
    <summary>Answer</summary>
    p(x) = 12x<sup>5</sup> − 30x<sup>4</sup> + 20x<sup>3</sup> − 1
  </details>
  <details>
    <summary>Hint</summary>
    <ul>
      <li>Polynomial Factor Theorem</li>
    </ul>
  </details>
   <br />

- [$\star\star\star$] If $r$ is a real number such that $r^3-r-1=0$ and $r+\sqrt{2}$ is a root of the polynomial $P(x)=0$, and if $p(x)$ is a polynomial with integer coefficients, a leading coefficient of $1$, and the least degree possible such that $p(x)$ satisfies the given conditions, Find $p(x)$.
  <details>
    <summary>Answer</summary>
    p(x) = x<sup>6</sup> − 8x<sup>4</sup> − 2x<sup>3</sup> + 13x<sup>2</sup> − 10x − 1
  </details>
   <br />

- [$\star$] Given that $f(x) = 1−x+x^2 −x^3 + \cdots −x^{19} +x^{20}$ is a polynomial with respect to $x$, and $g(y) = a_0+a_1y+ \cdots +a_{20}y_{20}$ is a polynomial with respect to $y$, where $y = x−4$, what's the value of $a_0+a_1+ \cdots +a_{20}$?
  <details>
    <summary>Answer</summary>
     1/6 * (5<sup>21</sup> + 1)
  </details>
   <br />

- [$\star\star\star$] Given that the first coefficient of a quintic polynomial $f(x)$ is $1$ and it satisfies $f(n) = 8n$ for $n = 1, 2, \cdots, 5$, what's the coefficient of the linear term of $f(x)$?
  <details>
    <summary>Answer</summary>
    282
  </details>
   <br />
