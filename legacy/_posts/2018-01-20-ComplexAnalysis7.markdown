---



layout: post



title :  (Complex Analysis) The zeta function and prime number theorem



date : 2018-01-20 09:52:04 +0900



---

(section 7) The zeta function and prime number theorem

(subsection 1) Zeros of zeta function

(prop) \zeta(s) = \prod_{p} \frac{1}{1-p^{-s}} . 

\zeta(s) = \pi^{s-1/2} \frac{\Gamma((1-s)/2)}{\Gamma(s/2)} \zeta(1-s)

(Thm 1.1.) The only zeros of \zeta outside the strip 0\le Re(s) \le 1 are at the negative even integers, -2,-4,-6,… The region that remains to be studied is called the critical strip.

(Def) Riemann Hypothesis : The zeros of \zeta(s) in the critical strip lie on the line Re(s) = 1/2.

the zeros of \zeta located outside the critical strip are sometimes called the trivial zeros of the zeta function.

(Thm 1.2.) The zeta function has no zeros on the line Re(s) = 1.

(Lem 1.3.) If Re(s) >1, then log \zeta(s) = \sum_{p,m} \frac{p^{-ms}}{m} = \sum_{n=1}^{\infty}c_{n}n^{-s} for some c_{n} \ge 0.

(Cor 1.5.) If \sigma >1 and t is real, then log|\zeta^{3}(\sigma) \zeta^{4}(\sigma + it) \zeta(\sigma + 2it)| \ge 0.

(subsection 1.1.) Estimates for 1/\zeta(s)

(prop 1.6.) For every \epsilon >0, we have 1/|\zeta(s)| \le c_{\epsilon} |t|^{\epsilon} when s = \sigma + it, \sigma \ge 1, and |t| \ge 1.

(section 2) Reduction to the functions \psi and \psi_{1}

(Def) Tchebychev’s \psi-function is defined by \psi(x) = \sum_{p^{m} \le x} log p.

(Prop 2.1.) If \psi(x) \sim x as x \to \infty, then \pi(x) \sim x/log x as x \to \infty.

(Prop 2.2.) If \psi_{1}(x) \sim x^{2}/2 as x \to \infty, then \psi(x) \sim x as x \to \infty, and therefore \pi(x) \sim x/log x as x \to \infty.

(Prop 2.3.) For all c > 1 \psi_{1} (x) = \frac{1}{2\pi i} \int_{c-i\infty}^{c + i\infty} \frac{x^{s+1}}{s(s+1)} (-\frac{\zeta’(s)}{\zeta(s)}) ds.

(Lem 2.4.) If c >0, then \frac{1}{2\pi i} \int_{c-i\infty}^{c + i\infty}\frac{a^{s}}{s(s+1)} ds = \begin{cases}0 & if 0 < a \le 1 \\ 1-1/a & if 1\le a. \end{cases}

Here, the integral is over the vertical line Re(s) = c.

(subsubsection 2.1.) Proof of the asymptotic for \psi_{1}

(prop) \psi_{1}(x) \sim x^{2}/2 as x \infty.

(subsubsection) Note on interchanging double sums. if {a_{kl}_{1\le k,l < \infty} is a sequence of complex numbers indexed by \mathbb{N} \times \mathbb{N}, s.t. \sum_{k=1}^{\infty} (\sum_{l=1}^{\infty} |a_{kl}|) <\infty, then

The double sum A = \sum_{k=1}^{\infty} (\sum_{l=1}^{\infty} a_{kl} ) summed in this order converges, and we may in fact interchange the order of summation, so that A = \sum_{k=1}^{\infty} \sum_{l=1}^{\infty} a_{kl} = \sum_{l=1}^{\infty} \sum_{k=1}^{\infty} a_{kl} .

Given \epsilon >0, there is a positive integer N so that for all K,L >N we have |A-\sum_{k=1}^{K} \sum_{l=1}^{L} a_{kl} | <\epsilon.

If m \mapsto (k(m), l(m)) is a bijection from \mathbb{N} to \mathbb{N} \times \mathbb{N}, and if we write c_{m} = a_{k(m)l(m)}, then A = \sum_{k=1}^{\infty} c_{k}.

 (Def) A bijective holomorphic function f : U \to V is called a conformal map or biholomorphism. Given such a mapping f, we say that U and V are conformally equivalent or simply biholomorphic.

(Prop 1.1.) If f : U \to V is holomorphic and injective, then f’(z) \neq 0 for all z \in U. In particular, the inverse of f defined on its range is holomorphic, and thus the inverse of a conformal map is also holomorphic.

(subsubseciton 1.1.) The disc and upper half-plane

(Def) The upper half-plane, which we denote by \mathbb{H}, consists of those complex numbers with positive imaginary part; that is, \mathbb{H} = {z \in \mathbb{C} : Im(z) >0}. 

(Thm 1.2.) The map F : \mathbb{H} \to \mathbb{D} : F(z) = \frac{i-z}{i+z} is a conformal map with inverse G : \mathbb{D} \to \mathbb{H} : G(w) = i\frac{1-w}{1+w}.

(Def) Mappings of the form z \mapsto \frac{az+b}{cz+d} where a,b,c, and d are complex numbers, and where the denominator is assumed not to be multiple of the numerator, are usualy referred to as fractional linear transformations.

(subsubsection 1.2.) Further examples

(Def) For any non-zero complex number c, the map f : z \mapsto cz is a conformal map from the complex plane to itself, whose inverse is simply g: w\mapsto c^{-1}w . If c has modulus 1, so that c = e^{i\varphi} for some real \varphi, then f is a rotation by \varphi. If c >0, then f corresponds to a dilation. 

(subsubsection 1.3.) The Dirichlet problem in a strip

(Def) The Dirichlet problem in the open set \Omega consists of solving \begin{cases} \Delta u = 0 & in \Omega \\ u = f & on \partial \Omega, \end{cases} where \Delta denotes the Laplacial \partial^{2}/\partial x^{2} + \partial^{2}/\partial y^{2} , and f is a given function on the boundary of \Omega .

(Lem 1.3.) Let V and U be open sets in \mathbb{C} and F : V \to U a holomorphic function. If u : U \to \mathbb{C} is a harmonic function, then u \bullet F is harmonic on V.

(subsection 2) The Schwarz lemma ; automorphisms of the disc and upper half-plane

(Lem 2.1.) Let f : \mathbb{D} \to \mathbb{D} be holomorphic with f(0) = 0. Then |f(z)| \le |z| for all z \in \mathbb{D}.

If for some z_{0} \neq 0 we have |f(z_{0})| = |z_{0}| , then f is a rotarion.

|f’(0)| \le 1, and if equality holds, then f is a rotation.

(subsubsection 2.1.) Automorphisms of the disc

(Def) A conformal map from an open set \Omega to itself is called an automorphism of \Omega. The set of all automorphisms of \Omega is denoted by Aut(\Omega), and carries the structure of a group.

if f and g are automorphisms of \Omega, then f \bullet g is also an automorphism.

(Thm 2.2.) If f is an automorphism of the disc, then there exist \theta \in \mathbb{R} and \alpha \in \mathbb{D} s.t. f(z) = e^{i\theta} \frac{\alpha - z}{1-\bar{\alpha} z}.

(Cor 2.3.) The only automorphisms of the unit disc that fix the origin are the rotations.

(subsubsection 2.2.) Automorphisms of the upper half-plane

(prop ) Aut(\mathbb{D}) and Aut(\mathbb{H}) are the same.

Aut(\mathbb{H}) consists of all maps z \mapsto \frac{az + b}{cz + d} where a,b,c and d are real numbers with ad – bc = 1. 

(Def) Let SL_{2} (\mathbb{R}) denote the group of all 2 \times 2 matrices with real entreis and determinant 1, namely SL_{2}(\mathb{R}) = {M = \begin{pmatrix}a & b \\ c & d \end{pmatrix} : a,b,c,d \in \mathbb{R} and det(M) = ad-bc = 1}. This group is called the special linear group.

Given a matrix M \in SL_{2}(\mathbb{R}) we define the mapping f_{M} by f_{M}(z) = \frac{az+b}{cz+d}.

(Thm 2.4.) Every automorphism of \mathbb{H} takes the form f_{M} for some M \in SL_{2}(\mathbb{R}) . Conversely, every map of this form is an automorphism of \mathbb{H}.

(Def) Since the two matrices M and -M give rise to the same function f_{M} = f_{-M}, if we identify the two matrices M and -M, then we obtain a new group PSL_{2}(\mathbb{R}) called the projective special linear group; which is isomorphic with Aut(\mathbb{H}) .

(subsection 3) The Riemann mapping theorem

(subsubsection 3.1.) Necessary conditions and statement of the theorem

(Def) Call a subset \Omega of \mathbb{C} proper if it is non-empty and not the whole of \mathbb{C} .

(Riemann mapping theorem) (Thm 3.1.) Suppose \Omega is proper and simply connected. If z_{0} \in \Omega, then there exists a unique conformal map F : \Omega \to \mathbb{D} s.t. F(z_{0}) = 0 and F’(z_{0}) >0. 

(Cor 3.2.) Any two proper simply connected open subsets in \mathbb{C} are comformally equivalent.

(subsubsection 3.2.) Montel’s theorem

(Def) Let \Omega be an open subset of \mathbb{C}. A family \mathcal{F} of holomorphic functions on \Omega is said to be normal if every sequence in \mathcal{F} has a subsequence that converges uniformly on every compact subset of \Omega.

The family \mathcal{F} is said to be uniformly bounded on compact subsets of \Omega if for each compact set K \subset \Omega there exists B >0 s.t. |f(z)| \le B for all z \in K and f \in \mathcal{F}.

The family \mathcal{F} is equicontinuous on a compact set K if for every \epsilon >0 there exists \delta >0 s.t. whenever z , w \in K and |z-w| < \delta then |f(z)_f(w)| < \epsilon for all f \in \mathcal{F}.

(Thm 3.3.) Suppose \mathcal{F} is a family of holomorphic functions on \Omega that is uniformly bounded on compact subsets of \Omega. Then

\mathcal{F} is equicontinuous on every compact subset of \Omega.

\mathcal{F} is a normal family.

(Def) A sequence {K_{l}}_{l=1}^{\infty} of compact subsets of \Omega is called an exhaustion if

K_{l} is contained in the interor of K_{l+1} for all l = 1,2,…

Any compact set K \subset \Omega is contained in K_{l} for some l. In particular \Omega = \bigcup_{l=1}^{\infty} K_{l}.

(Lem 3.4.) Any open set \Omega in the complex plane has an exhaustion.

(Prop 3.5.) If \Omega is a connected open subset of \mathbb{C} and {f_{n}} a sequence of injective holomorphic functions on \Omega that converges uniformly on every compact subset of \Omega to a holomorphic function f, then f is either injective or constant.

(subsubsection 3.3.) Proof of Riemann mapping theorem

(Def) \Omega is holomorphically simply connected if for any holomorphic function f in \Omega and any closed curve \gamma in \Omega, we have \int_{\gamma} f(z) dz = 0.

(subsection 4) Conformal mappings onto polygons

(subsubsection 4.2.) The Schwarz-Christoffel integral

(Def) The general Schwarz-Christoffel integral by S(z) = \int_{0}^{z} \frac{d\zeta}{(\zeta – A_{1})^{\beta_{1}}\cdot(\zeta – A_{n})^{\beta_{n}}}. Here A_{1} < A_{2} < \cdot < A_{n} are n distinct points on the real axis arranges in increasing order. The exponents \beta_{k} will be assumed to satisfy the conditions \beta_{k} <1 for each k and 1 < \sum_{k=1}^{n} \beta_{k}.

The integrand is defined as follows : (z-A_{k})^{\beta_{k}} is that branch (Defined in the complex plane slit along the infinite ray {A_{k} + iy : y \le 0}) which is positive when z = x is real and x > Z_{k} . As a result (z-A_{k})^{\beta_{k}} = \begin{cases} (x-A_{k})^{\beta_{k}} & if x is real and x > A_{k} \\ |x – A_{k}|^{\beta_{k}} e^{i\pi \beta_{k}} & if x is real and x < A_{k}.\end{cases}

(Prop 4.1.) Suppose S(z) is given as above.

If \sum_{k=1}^{n} \beta_{k} = 2, and \mathfrak{p} denotes the polygon whose vertices are given (in order) by a_{1}, …, a_{n}, then S maps the real axis onto \mathfrak{p} – {a_{\infty}}. The point a_{\infty} lies on the segment [a_{n}, a_{1}] and is the image of the point at infinity. Moreover, the (interior) angle at the vertex a_{k} is \alpha_{k} \pi where \alpha_{k} = 1- \beta_{k}.

There is a similar conclusion when 1< \sum_{k=1}^{n} \beta_{k} <2 except now the image of the extended line is the polygon of n+1 sides with vertices a_{1}, a_{2},… , a_{n} , a_{\infty}. The angle at the vertex a_{\infty} is \alpha_{\infty} \pi with \alpha_{\infty} = 1- \beta_{\infty}, where \beta_{\infty} = 2 - \sum_{k=1}^{n} \beta_{k}

(subsubsection 4.3.) Boundary behavior

(Def) a polygonal region P, namely a bounded, simply connected open set whose boundary is a polygonal line \mathfrak{p}. In this context, we always assume that the polygonal line is closed and we sometimes refer to \mathfrak{p} as a polygon.

(Thm 4.2.) If F : \mathbb{D} \to P is a conformal map, then F extends to a continuous bijection from the closure \bar{\mathbb{D}} of the disc to the closure \bar{P} of the polygonal region. In particular, F gives rise to a bijection from the boundary of the disc to the boundary polygon \mathfrak{p}.

(Lem 4.3.) For each 0 < r < 1/2, let C_{r} denote the circle centered at z_{0} of radius r. Suppose that for all sufficienctly small r we are given two points z_{r} and z’_{r} in the unit disc that also lie on C_{r}. If we let \rho(r) = |f(z_{r}) – f(z’_{r})| , then there exists a sequence {r_{n}} of radii that tends to zero, and s.t. \lim_{n \to \infty} \rho(r_{n}) = 0.

(Lem 4.4.) Let z_{0} be a point on the unit circle. Then F(z) tends to a limit as z approaches z_{0} within the unit disc.

(Lem 4.5.) The conformal map F extends to a continuous function from the closure of the disc to the closure of the polygon.

(subsubseciton 4.4.) The mapping formula

(Def) Suppose P is a polygonal region bounded by a polygon \mathfrak{p} whose vertices are ordered consecutively a_{1},a_{2},…,a_{n} and with n \ge 3. We denote by \pi \alpha_{k} the interior angle at a_{k}, and define the exterior angle \pi \beta_{k} by \alpha_{k} + \beta_{k} = 1. A simple geometric argument provides \sum_{k=1}^{n} \beta_{k} = 2.

(Thm 4.6.) There exist complex numbers c_{1} and c_{2} so that the conformal map F of \mathbb{H} to P is given by F(z) = c_{1}S(z) + c_{2} where S is the Schwarz-Christoffel integral introduced before.

(Thm 4.7.) If F is a conformal map from the upper half-plane to the polygonal region P and maps the points A_{1},…,A_{n-1}, \infty to the vertices of \mathfrak{p}, then there exists constants C_{1} and C_{2} s.t. F(z) = C_{1} \int_{0}^{z} \frac{d\zeta}{(\zeta – A_{1})^{\beta_{1}}\cdot(\zeta – A_{n-1})^{\beta_{n-1}}} + C_{2}.

(subsubsection 4.5.) Return to elliptic integrals

(Def) The elliptic integral I(z) = \int_{0}^{z} \frac{d \zeta}{[(1-\zeta^{2})(1-k^{2}\zeta^{2}]^{1/2}} with 0 < k < 1. 

(prop)it mapped the real axis to the rectangle R with vertices -K, K, K + i K’, and -K + iK’.

This mapping is a conformal mapping of \mathbb{H} to the interior of R.

