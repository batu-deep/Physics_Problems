# Section 0: Mathematical Foundations — Solutions

## 1. Vector Algebra  
Given \(\vec a=\langle 2,1,-3\rangle\), \(\vec b=\langle 4,-2,1\rangle\).

### a) Magnitudes
\[
|\vec a|=\sqrt{2^2+1^2+(-3)^2}=\sqrt{4+1+9}=\sqrt{14}
\]
\[
|\vec b|=\sqrt{4^2+(-2)^2+1^2}=\sqrt{16+4+1}=\sqrt{21}
\]

### b) Dot product
\[
\vec a\cdot \vec b = 2\cdot 4 + 1\cdot (-2) + (-3)\cdot 1 = 8-2-3=3
\]

### c) Cross product
\[
\vec a\times \vec b=
\begin{vmatrix}
\mathbf i & \mathbf j & \mathbf k\\
2&1&-3\\
4&-2&1
\end{vmatrix}
\]
\[
= \mathbf i(1\cdot 1-(-3)(-2))-\mathbf j(2\cdot 1-(-3)\cdot 4)+\mathbf k(2\cdot (-2)-1\cdot 4)
\]
\[
=\mathbf i(1-6)-\mathbf j(2-(-12))+\mathbf k(-4-4)
\]
\[
=\langle -5,-14,-8\rangle
\]

### d) Angle between \(\vec a\) and \(\vec b\)
\[
\cos\theta=\frac{\vec a\cdot \vec b}{|\vec a||\vec b|}=\frac{3}{\sqrt{14}\sqrt{21}}=\frac{3}{\sqrt{294}}
\]
\[
\theta=\cos^{-1}\!\left(\frac{3}{\sqrt{294}}\right)\approx 80.0^\circ
\]

---

## 2. Systems of Equations
\[
\begin{cases}
2x+3y=12\\
x-y=1
\end{cases}
\Rightarrow x=y+1
\]
Substitute:
\[
2(y+1)+3y=12 \Rightarrow 5y+2=12 \Rightarrow y=2
\]
\[
x=y+1=3
\]
**Answer:** \((x,y)=(3,2)\)

---

## 3. Proportionality (Gravitation)
\[
F = G\frac{m_1m_2}{r^2}
\]
If \(r\to 2r\), and \(m_1\to \frac{m_1}{2}\), \(m_2\to \frac{m_2}{2}\):
\[
F' = G\frac{(\frac{m_1}{2})(\frac{m_2}{2})}{(2r)^2}
=G\frac{\frac{m_1m_2}{4}}{4r^2}
=G\frac{m_1m_2}{16r^2}
=\frac{1}{16}F
\]
**Force becomes \(\boxed{\tfrac{1}{16}}\) of the original.**

---

## 4. Rearranging Formulas (Pendulum)
\[
T=2\pi\sqrt{\frac{L}{g}}
\]
Divide by \(2\pi\):
\[
\frac{T}{2\pi}=\sqrt{\frac{L}{g}}
\]
Square:
\[
\left(\frac{T}{2\pi}\right)^2=\frac{L}{g}
\]
Solve for \(g\):
\[
g=\frac{L}{(T/2\pi)^2}=\frac{4\pi^2 L}{T^2}
\]
**Answer:** \(\boxed{g=\frac{4\pi^2 L}{T^2}}\)

---

## 5. Trigonometry (Vector Components)
Magnitude \(A=15\), angle \(\theta=60^\circ\) from horizontal.
\[
A_x=A\cos\theta=15\cos 60^\circ=15\cdot \frac12=7.5
\]
\[
A_y=A\sin\theta=15\sin 60^\circ=15\cdot \frac{\sqrt3}{2}=\frac{15\sqrt3}{2}\approx 12.99
\]
**Components:** \(\boxed{(A_x,A_y)=\left(7.5,\frac{15\sqrt3}{2}\right)}\)

---

## 6. Function Analysis
\[
f(x)=3x^2-12x+7
\]
Differentiate:
\[
f'(x)=6x-12
\]
Critical point:
\[
6x-12=0 \Rightarrow x=2
\]
Second derivative:
\[
f''(x)=6>0
\]
So \(x=2\) is a **local minimum**.
\[
f(2)=3(4)-12(2)+7=12-24+7=-5
\]
**Local minimum:** \(\boxed{(2,-5)}\).  
**No local maximum** (parabola opens upward).

---

## 7. Logic & Series (Fly and Bicycle)
Bicycle is 10 m from wall, moves toward it at \(1\text{ m/s}\).  
Time until bicycle hits wall:
\[
t=\frac{10}{1}=10\text{ s}
\]
Fly flies the entire time at \(2\text{ m/s}\) (turnarounds don’t change total path length).
\[
\text{Distance} = vt = 2\cdot 10 = 20\text{ m}
\]
**Answer:** \(\boxed{20\text{ m}}\)

---

## 8. Definite Integrals
Area under \(f(x)=\sin x\) from \(0\) to \(\pi\):
\[
\int_0^\pi \sin x\,dx = \left[-\cos x\right]_0^\pi = (-\cos\pi)-(-\cos 0)= -(-1)-(-1)=1+1=2
\]
**Answer:** \(\boxed{2}\)

---

## 9. Optimization (Max Area Rectangle)
Rectangle under \(y=3-x^2\) in first quadrant, with upper-right corner at \((x,y)\) on curve.  
Then \(y=3-x^2\), width \(=x\), height \(=y\).
\[
A(x)=x(3-x^2)=3x-x^3,\quad 0\le x\le \sqrt3
\]
Differentiate:
\[
A'(x)=3-3x^2=3(1-x^2)
\]
Set to zero:
\[
1-x^2=0 \Rightarrow x=1 \quad (\text{first quadrant})
\]
Then
\[
y=3-1^2=2
\]
**Max-area rectangle dimensions:** \(\boxed{\text{width }1,\ \text{height }2}\)

---

## 10. Infinite Series (Ant’s Final Position)
Moves: \(1\) east, \(\frac12\) north, \(\frac13\) west, \(\frac14\) south, \(\frac15\) east, ...

### x-coordinate (east-west)
East steps: \(1+\frac15+\frac19+\cdots=\sum_{k=0}^\infty \frac{1}{4k+1}\)  
West steps: \(\frac13+\frac17+\frac{1}{11}+\cdots=\sum_{k=0}^\infty \frac{1}{4k+3}\)

Net:
\[
x=\sum_{k=0}^\infty\left(\frac{1}{4k+1}-\frac{1}{4k+3}\right)
=1-\frac13+\frac15-\frac17+\cdots
\]
This is the Gregory–Leibniz series:
\[
1-\frac13+\frac15-\frac17+\cdots=\frac{\pi}{4}
\]
So \(\boxed{x=\frac{\pi}{4}}\).

### y-coordinate (north-south)
North steps: \(\frac12+\frac16+\frac{1}{10}+\cdots=\sum_{k=0}^\infty \frac{1}{4k+2}\)  
South steps: \(\frac14+\frac18+\frac{1}{12}+\cdots=\sum_{k=0}^\infty \frac{1}{4k+4}\)

Net:
\[
y=\sum_{k=0}^\infty\left(\frac{1}{4k+2}-\frac{1}{4k+4}\right)
=\sum_{k=0}^\infty\left(\frac{1}{2(2k+1)}-\frac{1}{4(k+1)}\right)
\]
Compute by splitting:
\[
\sum_{k=0}^\infty \frac{1}{4k+2}=\frac12\sum_{k=0}^\infty\frac{1}{2k+1}
\]
\[
\sum_{k=0}^\infty \frac{1}{4k+4}=\frac14\sum_{k=1}^\infty\frac{1}{k}
\]
Using \(\sum_{k=0}^\infty \frac{1}{2k+1} = \sum_{k=1}^\infty\frac1k - \sum_{k=1}^\infty\frac{1}{2k}\),
this simplifies to:
\[
y=\frac14\left(\sum_{k=1}^\infty\frac1k-\sum_{k=1}^\infty\frac{1}{2k}\right)
=\frac14\left(H_\infty-\frac12H_\infty\right)
\]
More cleanly, recognize it as:
\[
y=\frac14\sum_{k=1}^\infty\frac{(-1)^{k-1}}{k}
=\frac14\ln 2
\]
So \(\boxed{y=\frac{\ln 2}{4}}\).

### Final position
\[
\boxed{\left(\frac{\pi}{4},\frac{\ln 2}{4}\right)}
\]

---
