# Section 0: Mathematical Foundations — Solutions

## 1. Vector Algebra
Given:
- a = [2, 1, -3]
- b = [4, -2, 1]

### a) Magnitudes
|a| = sqrt(2^2 + 1^2 + (-3)^2) = sqrt(4 + 1 + 9) = sqrt(14) ≈ 3.7417  
|b| = sqrt(4^2 + (-2)^2 + 1^2) = sqrt(16 + 4 + 1) = sqrt(21) ≈ 4.5826

### b) Dot product
a · b = 2*4 + 1*(-2) + (-3)*1 = 8 - 2 - 3 = 3

### c) Cross product
a x b = [
  a2*b3 - a3*b2,
  a3*b1 - a1*b3,
  a1*b2 - a2*b1
]

= [
  1*1 - (-3)*(-2),
  (-3)*4 - 2*1,
  2*(-2) - 1*4
]

= [ 1 - 6,  -12 - 2,  -4 - 4 ]
= [ -5, -14, -8 ]

### d) Angle between a and b
cos(theta) = (a · b) / (|a||b|) = 3 / (sqrt(14)*sqrt(21)) = 3 / sqrt(294)

sqrt(294) ≈ 17.146  
cos(theta) ≈ 3 / 17.146 ≈ 0.1749  
theta ≈ arccos(0.1749) ≈ 79.9 degrees


## 2. Systems of Equations
Solve:
- 2x + 3y = 12
- x - y = 1

From x - y = 1 => x = 1 + y

Substitute:
2(1 + y) + 3y = 12
2 + 2y + 3y = 12
5y = 10
y = 2

Then x = 1 + 2 = 3

Answer: x = 3, y = 2


## 3. Proportionality (Gravitation)
F = G * (m1*m2) / r^2

Changes:
- r is doubled: r' = 2r
- both masses are halved: m1' = m1/2, m2' = m2/2

New force:
F' = G * ((m1/2)(m2/2)) / (2r)^2
   = G * (m1*m2/4) / (4r^2)
   = G * (m1*m2) / (16r^2)
   = F / 16

Answer: Force becomes 1/16 of the original (decreases by factor 16).


## 4. Rearranging Formulas (Pendulum)
T = 2*pi * sqrt(L/g)

T / (2*pi) = sqrt(L/g)
(T / (2*pi))^2 = L/g
g = L / (T/(2*pi))^2 = (4*pi^2*L) / T^2

Answer: g = 4*pi^2*L / T^2


## 5. Trigonometry (Vector components)
Magnitude |A| = 15, angle theta = 60 degrees

Ax = 15*cos(60) = 15*(1/2) = 7.5
Ay = 15*sin(60) = 15*(sqrt(3)/2) ≈ 15*0.8660 ≈ 12.99

Answer: Ax = 7.5, Ay ≈ 12.99


## 6. Function Analysis
f(x) = 3x^2 - 12x + 7

Derivative:
f'(x) = 6x - 12

Critical point:
6x - 12 = 0 => x = 2

Second derivative:
f''(x) = 6 > 0  => local minimum

Value at x=2:
f(2) = 3*(4) - 12*(2) + 7 = 12 - 24 + 7 = -5

Answer: Local minimum at (2, -5). No local maximum.


## 7. Logic & Series (Fly and bicycle)
Bicycle is 10 m from wall, moves at 1 m/s toward wall.
Time to reach wall: t = 10 / 1 = 10 s

Fly moves continuously at 2 m/s for the same 10 s (instant turns don’t change total time).
Distance fly travels: d = v*t = 2*10 = 20 m

Answer: 20 m


## 8. Definite Integrals
Area under sin(x) from 0 to pi:

Integral of sin(x) dx = -cos(x)

∫[0..pi] sin(x) dx = (-cos(pi)) - (-cos(0))
= ( -(-1) ) - ( -(1) )
= 1 - (-1)
= 2

Answer: 2


## 9. Optimization Problem
Rectangle under y = 3 - x^2 in first quadrant.
Let top-right corner be (x, y) on curve, so y = 3 - x^2, with x >= 0.

Area:
A(x) = x*y = x(3 - x^2) = 3x - x^3

Derivative:
A'(x) = 3 - 3x^2

Set to zero:
3 - 3x^2 = 0 => x^2 = 1 => x = 1 (first quadrant)

Then y = 3 - 1^2 = 2

Answer: Maximum area rectangle has width = 1 and height = 2.


## 10. Infinite Series (Ant’s final position)
Moves:
1 east, 1/2 north, 1/3 west, 1/4 south, 1/5 east, ...

### x-position
x = 1 - 1/3 + 1/5 - 1/7 + 1/9 - ...
This is the alternating odd harmonic series:
1 - 1/3 + 1/5 - 1/7 + ... = pi/4

So x = pi/4 ≈ 0.7854

### y-position
y = 1/2 - 1/4 + 1/6 - 1/8 + 1/10 - ...
Factor 1/2:
y = (1/2) * (1 - 1/2 + 1/3 - 1/4 + 1/5 - ...)
The alternating harmonic series equals ln(2).

So y = (1/2)*ln(2) ≈ 0.3466

Final position:
(x, y) = (pi/4, (1/2)ln(2)) ≈ (0.7854, 0.3466)
