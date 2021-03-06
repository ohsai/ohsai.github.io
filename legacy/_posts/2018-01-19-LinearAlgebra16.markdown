---

layout: post

title : (Linear Algebra) Spectral Theorem

date : 2018-01-19 13:51:17 +0900

---

(Section 16) Spectral Theorem

(subsection 16.1) 표기법과 용어

(표기법 16.1.1.) 이 책에서 [T \in \mathfrak{LM}] 이라고 하면, 항상 [T \in \mathfrak{L}(V,V) 혹은 T \in \mathfrak{M}_{n,n}(F)] 를 뜻하기로 약속한다. 이때, dim V = n 이라고 놓자. 물론 T가 행렬이면 V = F^{n} 으로 이해하고, T = L_{T} 로 혼동한다. (즉, 행렬은 특수한 선형사상으로 이해한다.) 또, V \neq 0 이라고 가정한다.

(표기법 16.1.2.) F = \mathbb{C} 이고 (V,H) 가 non-degenerate Hermitian space 일 때, T = L \in \mathfrak{L}(V,V) 이면, T^{*} = L^{*} 로 이해한다. 따라서, T = A \in \mathfrak{M}_{n,n}(\mathbb{C}) 이면 T^{*} = (L_{A})^{*} 로 이해한다는 뜻이 된다.

(F에 제한은 없지만 대부분의 경우에 F = \mathbb{R} 이고, ) (V,B) 가 non-degenerate quadratic space 일 때에는, T = L \in \mathfrak{L}(V,V) 이면, T^{*} = ^{t}L 로 이해한다. 따라서, T = A \in \mathfrak{M}_{n,n}(F) 이면 T^{*} = ^{t}(L_{A}) 로 이해한다는 뜻이 된다. 그리고 quadratic space 임을 강조하기 위하여, T^{*} 보다는 ^{t}T 의 표기법을 더 자주 사용한다.

(관찰 16.1.4.) T \in \mathfrak{LM} 일 때, V의 subspace W 가 T-invariant 이고 동시에 T^{*}-invariant 이면, (T|_{W})^{*} = T^{*}|_{W} 이다.

(정의 16.1.5.) T \in \mathfrak{LM} 일 때

만약 [T^{*} = T] 이면, (V,H) 의 경우에는 T를 self-adjoint operator(또는, Hermitian operator) 라고 부르고, (V,B)의 경우에는 T를 symmetric operator 라고 부른다.

[T^{*} \cdot T = I] 이면 ,(V,H)의 경우에는 T를 unitary operator 라고 부르고, (V,B) 의 경우에는 T를 orthogonal operator 라고 부른다.

[T \cdot T^{*} = T^{*} \cdot T] 이면, T를 normal operator 라고 부른다.

(subsection 16.2.) Normal operator

(표기법 16.2.1.) 이 절에서는 항상 F = \mathbb{C} 이고, (V,\langle , \rangle ) 는 Hermitian inner product \langle, \rangle 가 주어진 n-차원 \mathbb{C}-vector space 이다.

(관찰 16.2.2.) T \in \mathfrak{LM} 이라고 할 때, [T의 eigen-vector 들로 이루어진 V의 orthonormal basis] 가 존재하려면, T는 normal 이어야만 한다.

(관찰 16.2.3.) T \in \mathfrak{LM} 일 때, 다음은 동치이다.

T 는 normal.

\langle Tv, Tw \rangle = \langle T^{*}v, T^{*}w \rangle for all v, w \in V.

(관찰 16.2.4.) T \in \mathfrak{LM} 이 normal이고, \lambda \in \mathbb{C} 이면, (T-\lambda I) 도 normal 이다.

(관찰 16.2.5) T \in \mathfrak{LM} 이 normal 일 때, Tv = \lambda v 이면 (단, 0 \neq v \in V, \lambda \in \mathbb{C}) , 즉 v가 eigen-value \lambda 를 갖는 T의 eigen-vector 이면, T^{*}v = \bar{\lambda} v 이다. 즉, v는 eigen-value \bar{\lambda} 를 갖는 T^{*} 의 eigen-vector 이다.

(Spectral Theorem ; positive definite Hermitian case) (정리 16.2.6.) T \in \mathfrak{LM} 일 때, 다음 조건은 동치이다.

T 는 normal.

[T의 eigen-vector 들로 이루어진 V의 orthonormal basis] 가 존재.

(정의 16.2.7.) The group of diagonal unitary matrices T_{U(n)} 을 T_{U(n)} = U(n) \cap D_{n}(\mathbb{C}) 로 정의한다. 그리고, T_{SU(n)} = SU(n) \cap D_{n}(\mathbb{C}) = T_{U(n)} \cap SL_{n}(\mathbb{C}) 로 정의한다.

(Spectral Theorem for U(n)) (따름정리 16.2.9.) 만약 A \in U(n) 이라고 하면, U^{-1}AU \in T_{U(n)} 인 U \in U(n) 이 존재한다. 따라서, U(n) = \bigcup_{U \in U(n)} U \cdot T_{U(n)} \cdot U^{-1} 로 쓸 수 있다.

(Spectral Theorem for SU(n)) (따름정리 16.2.10.) 만약 A \in SU(n) 이라고 하면, U^{-1}AU \in T_{SU(n)} 인 U \in SU(n) 이 존재한다. 따라서, SU(n) = \bigcup_{U \in SU(n)} U \cdot T_{SU(n)} \cdot U^{-1} 로 쓸 수 있다.

(subsection 16.3.) Symmetric Operator

(표기법 16.3.1.)이 절에서는 항상 F = \mathbb{R} 이고, (V,\langle , \rangle ) 는 inner product \langle, \rangle 가 주어진 n-차원 \mathbb{R}-vector space 이다. 그리고 T^{*} 보다 ^{t}T 를 더 많이 사용한다.

(명제 16.3.2.) T \in \mathfrak{LM} 이 symmetric operator 이면, T는 항상 (real) eigen-value 를 갖는다.

Symmetric matrix A \in \mathfrak{M}_{n,n}(\mathbb{R}) 은 항상 (real) eigen-value 를 갖는다.

(관찰 16.3.4.)T \in \mathfrak{LM} 이라고 할 때, [T의 eigen-vector 들로 이루어진 V의 orthonormal basis] 가 존재하려면 , T는 symmetric 이어야만 한다.

(Spectral Theorem ; positive definite real quadratic case) (정리 16.3.5.) T \in \mathfrak{LM} 일 때, 다음 조건은 동치이다.

T는 symmetric.

[T의 eigen-vector 들로 이루어진 V의 orthonormal basis] 가 존재.

(Spectral Therorem for real symmetric matrices) (따름정리 16.3.6.) \mathbb{R}^{n} 에 dot product 가 주어졌을 때, A \in \mathfrak{M}_{n,n}(\mathbb{R}) 이면, 다음 조건은 동치ㅣ다.

A는 symmetric matrix.

[A의 eigen-vector 들로 이루어진 \mathbb{R}^{n}의 orthonormal basis] 가 존재.

[U^{-1}AU 가 diagonal matrix] 인 U \in O(n) 이 존재.

(subsection 16.4.) Orthogonal Operator

(명제 16.4.1.) F = \mathbb{R} 이고, T \in \mathfrak{LM} 이면, [dim W = 1 혹은 dim W = 2] 인 V의 T-invariant subspace W 가 존재한다.

(Spectral Theorem for real orthogonal operators) (정리 16.4.2.) V를 inner product \langle , \rangle 가 주어진 finite dimensional \mathbb{R} – vector space 라 할때, T \in \mathfrak{LM} 이 orthogonal operator 이면, 다음 조건

V = W_{1} \oplus \cdots \oplus W_{s}.

W_{1}, …, W_{s} 는 V의 T-invariant subspace.

W_{1}, …., W_{s} 는 mutually orthogonal. 즉, W_{i} \perp W_{j} if i \neq j.

dim W_{i} = 1 or 2 for all i = 1,…,s 

를 만족하는 V의 subspace W_{1}, …, W_{s} 가 존재한다.

(표기법) B_{i} 가 square matrix들일 때, diag(B_{1}, …, B_{r}) 은 i-th diagonal block 에 B_{i} 가 있는 행렬, 즉 diag(B_{1}, ... , B_{r}) = \begin{pmatrix} B_{1} & 0 & \cdots & 0 \\ 0 & B_{2} & \cdots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \cdots & B_{r} \end{pmatrix} 을 의미하기로 한다.

(정의 16.4.3.) O(n) 의 subgroup T_{\mp} 를

n이 홀수이면 T_{\mp} = {diag(\mp 1, A_{1}, …, A_{r}) \in O(n) | A_{1}, …, A_{r} \in SO(2)} , 로 정의하고

n이 짝수이면 T_{\mp} = {diag(A_{0}, A_{1}, …, A_{r}) \in O(n) | A_{0} \in O(2) and A_{1}, …, A_{r} \in SO(2)} 로 정의한다.

(정의 16.4.4.) SO(n) 의 subgroup T_{SO(n)} 을 T_{SO(n)} = SO(n) \cap T_{\mp} 로 정의한다.

(Spectral Theorem for O(n)) (따름정리 16.4.6.) 만약 A \in O(n) 이라고 하면, U^{-1}AU \in T_{\mp} 인 U \in O(n) 이 존재한다. 따라서, O(n) = \bigcup_{U \in O(n)} U \cdot T_{\mp} \cdot U^{-1} 로 쓸 수 있다.

(Spectral Theorem for SO(n)) (따름정리 16.4.8.) A \in SO(n) 이라고 하면, U^{-1}AU \in T_{SO(n)} 인 U \in SO(n) 이 존재한다. 따라서, SO(n) = \bigcup_{U \in SO(n)} U \cdot T_{SO(n)} \cdot U^{-1} 로 쓸 수 있다.

(subsection 16.5.) Non-Degenerate Case

새로운 발상, 새로운 언어, 새로운 도구가 필요하다.

(subsection 16.6) Epilogue

(Schur’s Theorem) (정리 16.6.1.) F = \mathbb{C} 이고 (V , \langle , \rangle) 는 n-차원 Hermitian inner product space 라고 할 때, T \in \mathfrak{LM{ 이면 [T]_{\mathfrak{B}}^{\mathfrak{B}} 가 upper-triangular matrix 인 V의 orthonormal basis \mathfrak{B} 가 존재한다.

(정의 16.6.2.) (표기법 12.3.16) 의 abelian group \mathbb{Z}_{2} = {\bar{0}, \bar{1}} 에 다음과 같이 \bar{0} \cdot \bar{0} = \bar{0} \cdot \bar{1} = \bar{1} \cdot \bar{0} = \bar{0} , \bar{1} \cdot \bar{1} = \bar{1} 곱셈을 정의하면 \mathbb{Z}_{2} 는 field 가 된다.

(정의 16.6.3.) n-dimensional \mathbb{Z}_{2} -vector space (\mathbb{Z}_{2}^{n}) 의 \mathbb{Z}_{2}=subspace C 를 우리는 [linear (binary) code of length n] 이라고 부른다. 또, (\mathbb{Z}_{2}^{n})에 ‘보통 내적’ B_{\mathcal{E}}^{I} 가 주어졌다고 할때, C^{\perp} 를 C의 dual code 라고 부른다.

(정리 16.6.4.) C 가 (\mathbb{Z}_{2})^{n} 의 linear code 이면, dim C + dim C^{\perp} = n 이다. 따라서, dim C = m 이라고 하면, |C| = 2^{m} 이고, |C^{\perp}| = 2^{n-m} 이다.

