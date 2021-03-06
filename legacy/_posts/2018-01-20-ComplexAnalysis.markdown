---



layout: post



title : (Complex Analysis) Preliminaries to Complex Analysis



date : 2018-01-20 09:30:04 +0900



---

(Section 1) Preliminaries to Complex Analysis

(subsection 1) Complex numbers and the complex plane

(subsubsection) Basic Properties

(Def) A complex number takes the form z = x + iy where x and y are real. And i is an imaginary number that satisfies i^{2} = -1. We call x and y the real part and the imaginary part of z, and we write x = Re(z) and y = Im(z). A complex number with zero real part is said to be purely imaginary.

The set of all complex numbers is denoted by \mathbb{C}. The complex numbers can be visualized as the usual Euclidean plane : The complex number z = x + iy \in \mathbb{C} is identified with the point (x,y) \in \mathbb{R}^{2} .

x and y axis of \mathbb{R}^{2} are called the real axis and the imaginary axis.

(Def) If z_{1} = x_{1} + iy_{1} and z_{2} = x_{2} + iy_{2} , then z_{1} + z_{2} = (x_{1} + x_{2}) + i(y_{1} + y_{2}) and z_{1}z_{2} = (x_{1}x_{2} – y_{1}y_{2}) + i (x_{1}y_{2} + y_{1}x_{2}) .

Commutativity : z_{1} + z_{2} = z_{2} + z_{1} and z_{1}z_{2} = z_{2}z_{1} for all z_{1} , z_{2} \in \mathbb{C}.

Associativity : (z_{1} + z_{2}) + z_{3} = z_{1} + (z_{2} + z_{3}) ; and (z_{1}z_{2}) z_{3} = z_{1}(z_{2}z_{3}) for z_{1},z_{2},z_{3} \in \mathbb{C}.

Distributivity : z_{1}(z_{2}+z_{3}) = z_{1}z_{2} + z_{1}z_{3} for all z_{1}, z_{2}, z_{3} \in \mathbb{C}.

(Def) The absolute value of a complex number z = x + iy by |z| = (x^{2} + y^{2})^{1/2} , so that |z| is precisely the distance from the origin to the point (x,y). The triangle inequality |z+w| \le |z| + |w| for all z, w \in \mathbb{C}.

For all z \in \mathbb{C} we have both |Re(z)| \le |z| and |Im(z)| \le |z| , and for all z,w \in \mathbb{C}, ||z|-|w|| \le |z-w| .

The complex conjugate of z = x + iy is defined by \bar{z} = x – iy.

(prop) z is real iff z = \bar{z} and purely imaginary iff z = -\bar{z}.

Re(z) = \frac{z+\bar{z}}{2} and Im(z) = \frac{z-\bar{z}}{2i}.

\frac{1}{z} = \frac{\bar{z}}{|z|^{2}} whenever z \neq 0.

(Def) Polar form z = re^{i\theta} where r >0. Also \theta \in \mathbb{R} is called the argument of z and denoted by arg z. 

e^{i\theta} = cos \theta + i sin \theta.

If z = re^{i\theta} and w = se^{i\phi} , then zw = rs e^{i(\theta + \phi)}.

(subsubsection 1.2) Convergence 

(Def) A sequence {z_{1}, z_{2}, …} of complex numbers is said to converge to w \in \mathbb{C} if \lim_{n \to \infty| |z_{n} – w| = 0 , and we write w = \lim_{n \to \infty} z_{n}.

A sequence {z_{n}} is said to be a Cauchy sequence (or simply Cauchy) if |z_{n} – z_{m}| \to 0 as n , m \to \infty. In other words, given \epsilon >0 there exists an integer N>0 so that |z_{n} – z_{m}| < \epsilon whenever n,m >N.

(Prop) \mathbb{R} is complete : every Cauchy sequence of real numbers converges to a real number. The sequence {z_{n}} is Cauchy iff the sequences of real and imaginary parts of z_{n} are.

(Thm 1.1) \mathbb{C} , the complex numbers, is complete.

(subsubsection 1.3.) Sets in the complex plane

If z_{0} \in \mathbb{C} and r > 0 , we define the open disc D_{r}(z_{0}) of radius r centered at z_{0} to be the set of all complex numbers that are at absolute value strictly less than r from z_{0}. D_{r} (z_{0}) = {z \in \mathbb{C} : |z – z_{0}| < r}.

The closed disc \bar{D}_{r}(z_{0}) = {z \in \mathbb{C} : |z – z_{0}| < r} and the boundary of either the open or closed disc is the circle C_{r}(z_{0}) = {z \in \mathbb{C} : |z-z_{0}| = r.

Denote unit disc \mathbb{D} = {z \in \mathbb{C} : |z|<1}.

Given a set \Omega \subset \mathbb{C}, a point z_{0} is an interior point of \Omega if there exists r>0 s.t. D_{r}(z_{0}) \subset \Omega.

The interior of \Omega consists of all its interior points. A set \Omega is open if every point in that set is an interior point of \Omega. A set \Omega is closed if its complement \Omega^{c} = \mathbb{C} - \Omega is open. A point z \in \mathbb{C} is said to be a limit point of the set \Omega if there exists a sequence of points z_{n} \in \Omega s.t. z_{n} \neq z and \lim_{n \to \infty} z_{n} = z. The closure of any set \Omega is the union of \Omega and its limit points, and is often denoted by \bar{\Omega}.

Boundary of a set \Omega is equal to its closure minus its interior, and is often denoted by \partial \Omega. A set \Omega is bounded if there exists M>0 s.t. |z|<M whenever z \in \Omega. If \Omega is bounded, we define its diameter by diam(\Omega) = \sup_{z,w \in \Omega} |z-w|.

A set \Omega is said to be compact if it is closed and bounded.

(Thm 1.2.) The set \Omega \subset \mathbb{C} is compact iff every sequence {z_{n}} \subset \Omega has a subsequence that converges to a point in \Omega.

(Def) An open covering of \Omega is a family of open sets {U_{\alpha}} (not necessarily countable) s.t. \Omega \subset \bigcup_{\alpha} U_{\alpha}.

(Thm 1.3.) A set \Omega is compact iff every open covering of \Omega has a finite subcovering.

(prop 1.4.) If \Omega_{1} \supset \Omega_{2} \supset \cdots \supset \Omega_{n} \supset \cdots is a sequence of non-empty compact sets in \mathbb{C} with the property that diam(\Omega_{n}) \to 0 as n \to \infty, then there exists a unique point w \in \mathbb{C} s.t. w \in \Omega_{n} for all n.

(Def) An open set \Omega \subset \mathbb{C} is said to be connected if it is not possible to find two disjoint non-empty open sets \Omega_{1} and \Omega_{2} s.t. \Omega = \Omega_{1} \cap \Omega_{2}.

A connected open set in \mathbb{C} will be called a region. Similarly, a closed set F is connected if one cannot write F = F_{1} \cap F_{2} where F_{1} and F_{2} are disjoint non-empty closed sets.

(subsection 2) Functions on the complex plane

(subsubsection 2.1.) Continuous functions

(Def) Let f be a function defined on a set \Omega of complex numbers. We say that f is continuous at the point z_{0} \in \Omega if for every \epsilon >0 there exists \delta>0 s.t. whenever z \in \Omega and |z-z_{0}| < \delta then |f(z) – f(z_{0}) | < \epsilon.

(Prop) The function f is said to be continuous on \Omega if it is continuous at every point of \Omega. Sums and products of continuous functions are also continuous.

The function f of the complex argument z = x + iy is continuous iff it is continuous viewed as a function of the two real variables x and y.

(Def) f attains a maximum at the point z_{0} \in \Omega if |f(z)| \le |f(z_{0})| for all z \in \Omega, with the inequality reversed for the definition of a minimum.

(Thm 2.1.) A continuous function on a compact set \Omega is bounded and attains a maximum and minimum on \Omega.

(subsubsection 2.2.) Holomorphic functions

(Def) Let \Omega be an open set in \mathbb{C} and f a complex-valued function on \Omega. The function f is holomorphic at the point z_{0} \in \Omega if the quotient \frac{f(z_{0} + h) – f(z_{0})}{h} converges to a limit when h \to 0. The limit of the quotient, when it exists, is denoted by f’(z_{0}) , and is called the derivative of f at z_{0} ; f’(z_{0}) = \lim_{h \to 0} \frac{f(z_{0} + h) – f(z_{0})}{h}

(Def) The function f is said to be holomorphic on \Omega if f is holomorphic at every point of \Omega. If C is a closed subset of \mathbb{C}, we say that f is holomorphic on C if f is holomorphic in some open set containing C . Finally, if f is holomorphic in all of \mathbb{C} we say that f is entire.

The terms regular or complex differentiable or analytic are used instead of holomorphic occasionally.

(Prop) A function f is holomorphic at z_{0} \in \Omega iff there exists a complex number a s.t. f(z_{0} + h) – f(z_{0}) – ah = h \psi(h) , where \psi is a function defined for all small h and \lim_{h \to 0} \psi(h) = 0. f is continuous whenever it is holomorphic.

(Prop 2.2.) If f and g are holomorphic in \Omega, then 

f + g is holomorphic in \Omega and (f + g)’ = f’ + g’.

fg is holomorphic in \Omega and (fg)’ = f’g + fg’.

If g(z_{0}) \neq 0, then f/g is holomorphic at z_{0} and (f/g)’ = \frac{f’g – fg’}{g^{2}}. 

Moreover, if f : \Omega \to U and g : U \to \mathbb{C} are holomorphic, the chain rule holds

(g \bullet f)’(z) = g’(f(z))f’(z) for all z \in \Omega.

(Def) Let F(x,y) = (u(x,y), v(x,y)) . If F is differentiable, the partial derivative of u and v exist, and the linear transformation J is described in the standard basis of \mathbb{R}^{2} by the Jacobian matrix of F J = J_{F}(x,y) = \begin{pmatrix} \frac{\partial u}{\partial x} & \frac{\partial u}{\partial y } \\ \frac{\partial v}{\partial x} & \frac{\partial v}{\partial y}\end{pmatrix}

(Def) \frac{\partial u}{\partial x} = \frac{\partial v}{\partial y} and \frac{\partial u}{\partial y} = - \frac{\partial v}{\partial x} These are called Cauchy-Riemann equations.

(Def) \frac{\partial}{\partial z} = \frac{1}{2} (\frac{\partial}{\partial x} + \frac{1}{i} \frac{\partial}{\partial y} ) and \frac{\partial}{\partial \bar{z}} = \frac{1}{2} (\frac{\partial}{\partial x} - \frac{1}{i} \frac{\partial}{\partial y} )

(Prop 2.3.) If f is holomorphic at z_{0}, then \frac{\partial f}{\partial \bar{z}} (z_{0}) = 0 and f’(z_{0}) = \frac{\partial f}{\partial z} (z_{0}) = 2 \frac{\partial u}{\partial z} (z_{0}) . 

Also, if we write F(x,y) = f(z), then F is differentiable in the sense of real variables, and det J_{F} (x_{0}, y_{0}) = |f’(z_{0})|^{2}.

(Thm 2.4.) Suppose f = u + iv is a complex-valued function defined on an open set \Omega. If u and v are continuously differentiable and satisfy the Cauchy-Riemann equations on \Omega, then f is holomorphic on \Omega and f’(z) = \partial f / \partial z.

(subsection 2.3.) Power series

(Def) Complex exponential function which is defined for z \in \mathbb{C} by e^{z} = \sum_{n = 0}^{\infty} \frac{z^{n}}{n!} . This series converges absolutely for every z \in \mathbb{C}.

e^{z} is holomorphic in all of \mathbb{C}. e^{z} is its on derivative.

(Def) A power series is an expansion of the form \sum_{n = 0}^{\infty} a_{n} z^{n}.

(Thm 2.5.) Given a power series \sum_{n = 0}^{\infty} a_{n} z^{n}, there exists 0 \le R \le \infty s.t.

If |z| < R the series converges absolutely.

If |z| > R the series diverges.

Moreover, if we use the convention that 1/0 = \infty and 1/\infty = 0, then R is given by Hadamard’s formula 1/R = \limsum |a_{n}|^{1/n}.

The number R is called the radius of convergence of the power series, and the region |z|<R the disc of convergence. In particular, we have R = \infty in the case of exponential function, and R = 1 for the geometric series.

(Def) Trigonometric functions : cos z = \sum_{n = 0}^{\infty} (-1)^{n} \frac{z^{2n}}{(2n)!} and sin z = \sum_{n = 0}^{\infty} (-1)^{n} \frac{z^{2n+1}}{(2n+1)!}.

(Prop) cos z = \frac{e^{iz} + e^{-iz}}{2} and sin z = \frac{e^{iz} – e^{-iz}}{2i} These are called the Euler formulas for the cosine and sine functions.

(Thm 2.6.) The power series f(z) = \sum_{n = 0}^{\infty} a_{n}z^{n} defines a holomorphic function in its disc of convergence. The derivative of f is also a power series obtained by differentiating term by term the series for f, that is, f’(z) = \sum_{n = 0}^{\infty} nan_{n} z^{n-1}.

Moreover, f’ has the same radius of convergence as f.

(Cor 2.7.) A power series is infinitely complex differentiable in its disc of convergence, and the higher derivatives are also power series obtained by termwise differentiation.

(Def) A power series centered at z_{0} \in \mathbb{C} is an expression of the form f(z) = \sum_{n = 0}^{\infty} a_{n}(z – z_{0})^{n}. The disc of convergence of f is now centered at z_{0} and its radius is still given by Hadamard’s formula.

(Def) A function f defined on an open set \Omega is said to be analytic (or have a power series expansion) at a point z_{0} \in \Omega if there exists a power series \sum a_{n} (z-z_{0})^{n} centered at z_{0}, with positive radius of convergence, s.t. f(z) = \sum_{n = 0}^{\infty} a_{n}(z-z_{0})^{n} for all z in a neighborhood of z_{0}. 

If f has a power series expansion at every point in \Omega, we say that f is analytic on \Omega.

(subsection 3) Integration along curves

(Def) A parametrized curve is a function z(t) which maps a closed interval [a,b] \subset \mathbb{R} to the complex plane.

(Def) We say that the parametrized curve is smooth if z’(t) exists and is continuous at [a,b] , and z’(t) \neq 0 for t \in [a,b] . At the points t = a and t = b, the quantities z’(a) and z’(b) are interpreted as the one-sided limits z’(a) = \lim_{h \to 0 , h >0} \frac{z(a+h) – z(a)}{h} and z’(b) = \lim_{h \to 0, h < 0} \frac{z(b+h) – z(b)}{h}

(Def) We say that the parametrized curve is piecewise-smooth if z is continuous on [a,b] and if there exist points a = a_{0} < a_{1} < \cdots < a_{n} = b, where z(t) is smooth in the intervals [a_{k}, a_{k+1}] . 

The right-hand derivative at a_{k} may differ from the left-hand derivative at a_{k} for k = 1,…,n-1.

(Def) Two parametrizations, z : [a,b] \to \mathbb{C} and \tilde{z} : [c,d] \to \mathbb{C} are equivalent if there exists a continuously differentiable bijection s \mapsto t(s) from [c,d] \to [a,b] so that t’(s) >0 and \tilde{z}(s) = z(t(s)).

(Def) The family of all paramterizations that are equivalent to z(t) determines a smooth curve \gamma \subset \mathbb{C} , namely the image of [a,b] under z with the orientation given by z as t travels from a to b. define a curve \gamma^{-} obtained from the curve \gamma by reversing the orientation.

(Def) It is clear how to define a piecewise-smooth curve. The points z(a) and z(b) are called the end-points of the curve and are independent on the parametrization. Since \gamma carries an orientation, it is natural to say that \gamma begins at z(a) and ends at z(b).

(DeF) A smooth or piecewise smooth curve is closed if z(a) = z(b) for any of its parametrizations. Finaly, a smooth or piecewise-smooth curve is simple if it is not self-intersecting, that is, z(t) \neq z(s) unless s = t. 

(Def) For brevity, call any piecewise-smooth curve a curve.

(Def) The positive orientation(counterclockwise) is the one that is given by the standard parametrization z(t) = z_{0} + re^{it} , where t \in [0,2\pi], while the negative orientation(clockwise) is given by z(t) = z_{0} + re^{-it} , where t \in [0,2\pi].

Denote C a general positively oriented circle.

(Def) Given a smooth curve \gamma in \mathbb{C} parametrized by z : [a,b] \to \mathbb{C} , and f a continuous function on \gamma, we define the integral of f along \gamma by \int_{\gamma} f(z) dz = \int_{a}^{b} f(z(t)) z’(t) dt.

(Def) If \gamma is piecewise smooth, if z(t) is a piecewise-smooth parametrization as before, then \int_{\gamma} f(z)dz = \sum_{k = 0}^{n-1} \int_{a_{k}}^{a_{k+1}} f(z(t))z’(t) dt.

(Def) The length of the smooth curve \gamma is length(\gamma) = \int_{a}^{b} |z’(t)| dt.

(Prop 3.1.) Integration of continuous functions over curves satisfies the following properties : 

It is linear, that is if \alpha, \beta \in \mathbb{C}, then \int_{\gamma} (\alpha f(z) + \beta g(z)) dz = \alpha \int_{\gamma} f(z)dz + \beta \int_{\gamma} g(z) dz.

If \gamma^{-} is \gamma with the reverse orientation, then \int_{\gamma} f(z) dz = - \int_{\gamma^{-}} f(z) dz.

One has the inequality |\int_{\gamma} f(z) dz | \le \sup_{z \in \gamma} |f(z)} \cdot length(\gamma).

(Def) Suppose f is a function on the open set \Omega. A primitive for f on \Omega is a function F that is holomorphic on \Omega and s.t. F’(z) = f(z) for all z \in \Omega.

(Thm 3.2.) If a continuous function f has a primitive F in \Omega, and \gamma is a curve in \Omega that begins at w_{1} and ends at w_{2}, then \int_{\gamma} f(z) dz = F(w_{2}) – F(w_{1}) .

(Cor 3.3.) If \gamma is a closed curve in an open set \Omega, and f is continuous and has a primitive in \Omega, then \int_{\gamma} f(z)dz = 0.

(Cor 3.4.) IF f is holomorphic in a region \Omega and f’ = 0, then f is constant.

(Def) f(z) = O(g(z)) to mean that there is a constant C > 0 s.t. |f(z)| \le C|g(z)| for z in a neighborhood of the point in question. In addition, we say f(z) = o(g(z)) when |f(z)/g(z) | \to 0. We also write f(z) \simeq g(z) to mean that f(z)/g(z) \to 1.

