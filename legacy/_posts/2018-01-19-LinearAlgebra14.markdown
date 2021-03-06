---

layout: post

title : (Linear Algebra) Bilinear Form

date : 2018-01-19 13:51:15 +0900

---

(Section 14) Bilinear form

(subsection 14.1) Bilinear form

(정리 14.1.6.) \mathfrak{B} 를 n-dimensional F-vector space V 의 고정된 기저라고 할 때, 함수 \Omega_{\mathfrak{B}} : \mathfrak{Bil}(V) \to \mathfrak{M}_{n,n}(F) 를 \Omega_{\mathfrak{B}}(B) = [B]_{\mathfrak{B}} , (B \in \mathfrak{Bil}(V)) 로 정의하면 \Omega_{\mathfrak{B}} 는 vector space isomorphism 이다. 이때, [B]_{\mathfrak{B}} 를 (기저 \mathfrak{B} 에 관한) B의 행렬이라고 부른다.

(관찰 14.1.8.) F^{n} 에 bilinear form B_{\mathcal{E}}^{J} 가 주어져 있다고 하자. J 가 가역일 때, A \in \mathfrak{M}_{n,n}(F) 이면 B_{\mathcal{E}}^{J}(AX,Y) = B_{\mathcal{E}}^{J}(X,(J^{-1} \cdot ^{t}A \cdot J) Y ), (X,Y \in F^{n})

(정의 14.1.9.) B : V \times V \to F 가 F-vector space V 의 bilinear form 일 때,

B가 다음 조건 B(v,w) = B(w,v) (v,w \in V) 를 만족하면, B를 symmetric bilinear form 이라고 부른다.

B가 다음 조건 B(v,v) = 0 (v \in V) 를 만족하면, B를 alternating bilinear form 이라고 부른다.

(관찰 14.1.10.) \mathfrak{B} 가 f.d.v.s. V의 기저이고, B 가 V의 bilinear form 일 때, B가 symmetric 이기 위한 필요충분조건은 [B]_{\mathfrak{B}} 가 symmetric matrix 인 것이다.

(subsection 14.2.) 

(정의 14.2.2.) 유한차원 벡터공간 V위에 정의된 함수 Q : V \to F 가 다음 조건을 만족하면, Q를 V의 quadratic form 이라고 부른다.

B_{Q} : V \times V \to F 를 B_{Q} (v,w) = Q(v + w) -Q(v) – Q(w) (v,w \in V) 로 정의하면, B_{Q} 는 V의 symmetric bilinear form.

v \in V, c \in F 이면, Q(cv) = c^{2}Q(v)

따라서, quadratic form 이 주어지면, symmetric bilinear form 이 주어진다. 그리고, 그 역도 성립한다.

(관찰 14.2.4.) V가 유한차원 벡터공간을 때, 다음 대응관계 Q \leftrightarrow B_{Q} 는 [V의 quadratic form 전체의 집합] 과 [V의 symmetric bilinear form 전체 집합] 사이의 bijection 이다.

(정의 14.2.5.) 유한차원 벡터공간 V에 symmetric bilinear form B 가 주어졌다고 하자. 그러면, 앞 (관찰 14.2.4.) 에 의해, V의 quadratic form Q도 자동적으로 주어진다. 이 때, (V,B) = (V,B,Q) 를 quadratic space 라고 한다.

(section 14.3.) Orthogonal group 과 Symplectic group

(정의 14.3.1.) Quadratic space (V,B) 가 주어졌을 때 (따라서, B는 symmetric bilinear form 이고, quadratic form Q는 자동으로 주어져있다), O(V,B) = {L \in GL(V) | B(Lv, Lw) = B(v,w) for all v, w \in V} 로 정의하고, O(V,B) 를 (V,B) 로부터 만들어진 orthogonal group 이라고 부른다. 또, O(V,B) 의 원소는 물론 orthogonal operator 라고 부른다. 그리고, (V,B) 와 O(V,B) 를 공부하는 것을 orthogonal geometry 라고 부른다.

(명제 14.3.5.) \mathfrak{B} 를 quadratic space (V,B) 의 basis 라고 할 때, J = [B]_{\mathfrak{B}} 로 표기하면 (따라서 , J는 symmetric)

{[L]_{\mathfrak{B}}^{\mathfrak{B}} \in GL_{n}(F) | L \in O(V,B)} = {A \in GL_{n}(F) | ^{t}A \cdot J \cdot A = J} 이다.

(정의 14.3.6.) J \in \mathfrak{M}_{n,n}(F) 가 symmetric matrix 일 때, O_{n}^{J}(F) = {A \in GL_{n}(F) } ^{t}A \cdot J \cdot A = J} 로 표기하고, J에 대응하는 orthogonal group 이라고 부른다.

(정의 14.3.8.) B가 유한차원 벡터공간 V의 alternating bilinear form일 때, Sp(V,B) = {L \in GL(V) | B(Lv, Lw) = B(v,w) for all v , w \in V} 로 정의하고, Sp(V,B) 를 (V,B) 로부터 만들어진 symplectic group 이라고 부른다. 그리고 (V,B) 와 Sp(V,B) 를 공부하는 것을 symplectic grometry 라고 부른다.

(명제 14.3.9.) B가 유한차원 벡터공간 V의 alternating bilinear form 이고 , \mathfrak{B} 가 V의 기저일 때, J = [B]_{\mathfrak{B}} 로 표기하면 (따라서 ,J 는 skew-symmetric)

{[L]_{\mathfrak{B}}^{\mathfrak{B}} \in GL_{n}(F) | L \in Sp(V,B) } = {A \in GL_{n}(F) | ^{t}A \cdot J \cdot A = J} 이다.

(정의 14.3.10.) J \in \mathfrak{M}_{n,n}(F) 가 skew-symmetric matrix 일 때, SP_{n}^{J}(F) = {A \in GL_{n}(F) | ^{t}A \cdot J \cdot A = J} 로 표기하고, J에 대응하는 symplectic group 이라고 부른다.

(subsection 14.4.) O(1,1) 과 O(3,1)

(표기법) F = \mathbb{R}, J = diag(1,-1) 이라고 하면 \mathbb{R}^{2} 의 symmetric bilinear form B_{\mathcal{E}}^{J} 는 B_{\mathcal{E}}^{J} (\binom{a}{b} , \binom{c}{d} ) = ac – bd , (a,b,c,d \in \mathbb{R}) 로 주어질 것이다. 이 때, B_{\mathcal{E}}^{J} 에 대응하는 orthogonal group 을 O(1,1) = O_{2}^{J} (\mathbb{R}) = {A \in GL_{2}(\mathbb{R}) |^{t} A \cdot J \cdot A = J} 로 표기하자.

(정의 14.4.7.) J = diag(1,1,1,-1) 일 때, O(3,1) = O_{4}^{J}(\mathbb{R}) = {A \in GL_{4}(\mathbb{R}) | ^{t}A \cdot J \cdot A = J} 로 표기하고, O(3,1) 을 Lorenz group 이라고 부른다.

(subsection 14.5.) Non-degenerate Symmetric Bilinear form

(정의 14.5.1.) v, w \in V 일 때, B(v,w) = 0 이면 v \perp w 로 표기하고, v와 w 는 서로 수직이라고 말한다. 또, S,T \subseteq V 일 때, [B(v,w) = 0 for all v \in S, w \in T] 이면, S \perp T 라고 표기하고 S와 T는 서로 수직이라고 말한다.

(정의 14.5.3.) V의 basis \mathfrak{B} = {v_{i}} 가 mutually perpendicular subset 이면, \mathfrak{B} 를 V의 orthogonal basis 라고 부른다. 또, V의 orthogonal basis \mathfrak{B} = {v_{i}} 가 unit vector 들로 이루어져 있으면 (즉 ,B(v_{i}, v_{i}) = 1 for all i 이면) , \mathfrak{B} 를 V의 orthonormal basis 라고 부른다.

(표기법 14.5.5.) S \subseteq V 일 때, S^{\perp} = {v \in V | v \perp w for all w \in S} 로 표기한다.

(정의 14.5.9.) V^{\perp} = 0일 때, 우리는 B를 non-degenerate symmetric bilinear form 이라고 부른다.

(명제 14.5.11.) \mathfrak{B} 가 V의 basis 일 때, 다음은 동치이다.

B는 non-degenerate.

det([B]_{\mathfrak{B}}) \neq 0.

(정리 14.5.12.) B가 non-degenerate 일 때, W \le V 이면 dim W^{\perp} = dim V – dim W 가 성립한다.

(관찰 14.5.13.) [B(v,v) = 0 for all v \in V] 이면, B = 0 이다.

(보조정리 14.5.14.) w \in V 이고 B(w,w) \neq 0 이면, V = \langle w \rangle \oplus \langle w \rangle^{\perp} 이 성립한다.

(정리 14.5.15.) 모든 quadratic space (V,B) 는 orthogonal basis 를 갖는다. (물론 V \neq 0). (B 가 non-degenerate 일 필요도 없다.)

(정의 14.5.16.) 만약 , w \in V 가 B(w,w) \neq 0 을 만족하면, 함수 S_{w} : V \to V 를 S_{w}(v) = v - \frac{2B(v,w)}{B(w,w)} w, (v \in V) 라 정의하고, S_{w} 를 w에 관한 reflection 또는 symmetry 라고 부른다.

(subsection 14.6.) Dual space 와 Dual map

(명제 14.6.1.) 함수 \psi^{V} : V \to V^{**} 를 (\psi^{V}(v))(f) = f(v) , (v \in V , f \in V^{*}) 로 정의하면, \psi^{V} 는 vector space isomorphism 이다. 이 때, \psi^{V} 는 [기저의 선택과 무관한 natural isomorphism] 이므로, 우리는 \psi^{V} 를 사용해 V와 V^{**} 를 identify 한다.

(관찰 14.6.2.) v \in V 일 때, [f(v) = 0 for all f \in V^{*}] 이면, v = 0 이다.

(관찰 14.6.3.) {v_{1}, …, v_{n}} 이 f.d.v.s. V의 기저이면, \psi^{V}(v_{i}) = v_{i}^{**} (i = 1,…,n) 이 성립한다. (단, v_{i}^{**} = (v_{i}^{*})^{*} ).

(정의 14.6.5.) V,W 가 vector space 이고 L : V \to W 가 linear map 일 때, linear map L^{*} : W^{*} \to V^{*} 를 L^{*}(f) = f \bullet L , (f \in W^{*}) 으로 정의하고, L^{*} 를 L의 dual map 이라고 부른다.

(관찰 14.6.7.) \mathfrak{B} = {v_{1}, …, v_{n}} 을 V의 기저라고 하고, \mathfrak{C} = {w_{1}, …, w_{m}} 은 W의 기저라고 하자. 이 때, L \in \mathfrak{L}(V,W) 이면 [L^{*}]_{\mathfrak{B}^{*}}^{\mathfrak{C}^{*}} = ^{t}([L]_{\mathfrak{C}}^{\mathfrak{B}}) 가 성립한다.

(subsection 14.7.) Duality

(표기법) F-벡터공간 V 와 그 dual V^{*} 에 대해 bilinear form \epsilon : V \times V^{*} \to F : \epsilon(v,f) = f(v) , (v \in V, f \in V^{*}) 로 정의한다. S \subseteq V , T \subseteq V^{*} 일 때, S^{perp} = {f \in V^{*} | \epsilon(v,f) = 0 for all v \in S} , T^{perp} = {v \in V | \epsilon(v,f) = 0 for all f \in T} , 로 표기한다.

(정리 14.7.3.) V가 유한차원이고, W \le V, Y \le V^{*} 이면 다음이 성립한다.

dim W^{perp} = dim V – dim W.

dim Y^{perp} = dim V – dim Y.

(따름정리 14.7.4.) V가 유한차원이고, Y \le V^{*} 라고 하자. 만약, Y \neq V^{*} 이면, [f(v) = 0 for all f \in Y] 인 0 \neq v \in W 가 존재한다.

(subsection 14.8.) B-identification

(정리 14.8.1.) 함수 \phi^{V} = \phi_{B}^{V} : V \to V^{*} 를 (\phi^{V}(v))(w) = B(w,v) , (v,w \in V) 로 정의하면, \phi^{V} 는 linear map 이다. 이 때, 다음 조건은 동치이다.

B는 non-degenerate symmetric bilinear form.

\phi^{V} 는 monomorphism.

\phi^{V} 는 isomorphism.

V^{*} 의 모든 원소는 \phi^{V} (v) 의 꼴. (단, v \in V).

(관찰 14.8.3.) \mathfrak{B} 가 V의 기저이고, \mathfrak{B}^{*} 를 \mathfrak{B} 의 dual basis 라고 하면, [\phi_{B}^{V}]_{\mathfrak{B}^{*}}^{\mathfrak{B}} = [B]_{\mathfrak{B}}.

(표기법 14.8.4.) (V,B) 가 유한차원 non-degenerate quadratic space 일 때, (정리 14.8.1.) 의 isomorphism \phi^{V} 는 기저의 선택과 무관한 natural isomorphism 이다. 따라서 이번에도 \phi^{V} 를 통하여 V 와 V^{*} 를 identify 하고, V = V^{*} 로 표기법을 남용한다. 이를 B-identification 이라고 한다. 그리고, 혼동의 가능성이 없다면 \phi_{B}^{V} (v) = \phi_{v} (v \in V) 로 간략히 표기하기로 한다.

(명제 14.8.9.) (V,B) 가 유한차원 non-degenerate quadratic space 일 때, 함수 I \times \phi_{B}^{V} : V \times V \to V \times V^{*} 를 (I \times \phi_{B}^{V})(v,w) = (v, \phi_{w}) (v,w \in V) 로 정의하면, 다음 사각형 diagram 

\begin{tikzpicture} \matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] { V \times V & F\\ V \times V^{*} & F \\}; \path[-stealth] (m-1-1) edge node [left] {$I \times \phi_{B}^{V} $} node [right] {$=$} (m-2-1)  edge node [above] {$B$} (m-1-2) (m-1-2) edge node [right] {$ I $} node [left] {$=$} (m-2-2) (m-2-1) edge node [below] {$\epsilon$} (m-2-2);\end{tikzpicture}

은 commutative diagram 이다. 즉, B-identification 의 관점에서는 B = e 이다. (따라서, “\perp = perp “ 라고 말할 수 있다.)

(정리 14.8.10.) (V,B) 를 유한차원 non-degenerate quadratic space 라고 하고, W \le V 라고 하자. 그러면, B-identification 의 관점에서는 W^{\perp} = W^{perp} 이다. 특별히, dim W^{\perp} = dim V – dim W 이다.

(subsection 14.9.) Transpose Operator

(정의 14.9.1) L \in \mathfrak{L}(V,W) 라고 하자. 이때, 선형사상 L의 (B와 C에 관한) transpose map ^{t}L \in \mathfrak{L}(V,W) 는 – B-identification 과 C-identification 의 관점에서 - ^{t}L = L^{*} 로 정의된다. (L^{*} 는 L의 dual map) . 즉, ^{t}L : W \to V 는 다음 사각형 diagram 

\begin{tikzpicture} \matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] { W & V\\ W^{*} \times V^{*} & F \\}; \path[-stealth] (m-1-1) edge node [left] {$ \phi_{C}^{W} $} node [right] {$=$} (m-2-1)  edge node [above] {$^{t}L$} (m-1-2) (m-1-2) edge node [right] {$ \phi_{B}^{V} $} node [left] {$=$} (m-2-2) (m-2-1) edge node [below] {$L^{*}$} (m-2-2);\end{tikzpicture}

을 commutative diagram 으로 만들어주는 유일한 linear map 이다. 이를 식으로 표현한다면, ^{t}L = (\phi_{B}^{V})^{-1} \bullet L^{*} \bullet \phi_{C}^{W} 가 된다.

L \in \mathfrak{L}(V,V) 일 때 T의 transpose operator ^{t}L 을 ^{t}L = (\phi_{B}^{V})^{-1} \bullet L^{*} \bullet \phi_{B}^{W} 로 정의한다.

(관찰 14.9.2.) L,M \in \mathfrak{L}(V,V) 일 때, B(Lv, w) = B(Mv,w) , (v, w \in V) 이면, L = M 이다. (뒷자리에서도 마찬가지다.)

(명제 14.9.3.) L \in \mathfrak{L}(V,W) 이면, ^{t}L 은 다음 조건 C(Lv, w) = B(v, ^{t}Lw) , (v \in V , w \in W) 를 만족하는 유일한 linear map 이다. (B,C 는 symmetric 이므로, 이 조건은 C(w,Lv) = B(^{t}Lw, v) , (v \in V, w \in W) 와 동치이다.)

(명제 14.9.4.) \mathfrak{B,C} 를 각각 V,W의 고정된 기저라고 하자.

L \in \mathfrak{L}(V,W) 일 때, J_{\mathfrak{B}} = [B]_{\mathfrak{B}} , J_{\mathfrak{C}} = [C]_{\mathfrak{C}} 로 표기하면, [^{t}L]_{\mathfrak{B}}^{\mathfrak{C}} = (J_{\mathfrak{B}})^{-1} \cdot ^{t} ([L]_{\mathfrak{C}}^{\mathfrak{B}}) \cdot J_{\mathfrak{C}} 이다.

특별히, L \in \mathfrak{L}(V,V) 일 때, J = [B]_{\mathfrak{B}} 로 표기하면, [^{t}L]_{\mathfrak{B}}^{\mathfrak{B }} = J^{-1}\cdot ^{t} ([L]_{\mathfrak{B}}^{\mathfrak{B}}) \cdot J 이다.

(명제 14.9.6.) O(V,B) = {L \in GL(V) | ^{t}L \bullet L = I} .

(관찰 14.9.8.) t : \mathfrak{L}(V,W) \to \mathfrak{L}(W,V) 를 t(L) = ^{t}L (L \in \mathfrak{L}(V,V)) 로 정의하면, t 는 isomorphism 이다. 특별히, 다음이 성립한다.

L, M \in \mathfrak{L}(V,W) 이면, ^{t}(L+M) = ^{t}L + ^{t}M

L \in \mathfrak{L}(V,W), c \in F 이면, ^{t}(cL) = c \cdot ^{t}L.

(관찰 14.9.9.) 다음이 성립한다.

^{t}I = I.

L \in \mathfrak{L}(V,W) 이고 M \in \mathfrak{L}(W,U) 이면, ^{t}(M \bullet L) = ^{t}L \bullet ^{t}M.

L \in \mathfrak{L}(V,W) 이면, ^{t}(^{t}L) = L.

