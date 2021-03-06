---
layout: post
title : (Linear Algebra) Fundamental Theorem 기본정리
date : 2018-01-19 13:51:07 +0900
---
(Section 5) 기본정리

(subsection 5.1) Vector space of linear maps

(정의 5.1.1) V,W 가 F-vector space 일 때, \\(\mathfrak{L} (V,W) = {L : V \to W | L 은 linear map}\\( 으로 정의한다. 그리고, [\\(L,M \in \mathfrak{L}(V,W)\\) 의 합\\( L + M\\) ] 과, [scalar \\(a \in F\\) 와\\(L \in \mathfrak{L}(V,W)\\) 의 상수곱 \\(aL\\)] 을 각각 \\((L + M) (v) = L(v) + M(v) , (aL)(v) = aL(v) (v \in V)\\) 로 정의하면 \\(\mathfrak{L} (V,W)\\) 도 벡터공간이 된다.

(정의 5.1.5) V가 벡터공간일 때, \\(V^{*} = \mathfrak{L} (V,F)\\) 로 정의하고, 우리는 \\(V^{*}\\) 를 V 의 dual space (쌍대공간) 이라고 부른다. 또, \\(V^{*}\\) 의 원소는 linear functional 이라고 부른다. 뿐만 아니라, 우리는 dual 의 dual , 즉 \\((V^{*})^{*} = V^{**} = \mathfrak{L}(V^{*} , F)\\) 도 생각하게 된다. \\(V^{**}\\) 는 V의 double dual 이라고 부른다.

(관찰 5.1.7) V가 f.d.v.s. 이면, \\(dim V^{*} = dim V\\) 이다.

(정의 5.1.8) f.d.v.s V 에 대해 우선\\( \mathfrak{B} = {v_{1}, …, v_{n}}\\) 을 V의 기저라고 하자. \\(v_{i}^{*}  \in V^{*} 를 v_{i}^{*} (v_{j}) = \delta_{ij} (1 \le i,j \le n )\\) 이라 정의한다. 이제 \\(\mathfrak{B}^{*} = {v_{1}^{*} , …, v_{n}^{*}}\\) 가 \\(V^{*}\\) 의 basis 이다. 이 \\(\mathfrak{B}^{*} = {v_{1}^{*} , …, v_{n}^{*}}\\) 를 \\(\mathfrak{B}\\) 의 dual basis 라 부른다.

(관찰 5.1.9) V,W 가 f.d.v.s. 이면, \\(dim \mathfrak{L} (V,W) = (dim V) \cdot (dim W)\\) 이다.

(subsection 5.2.) 기본정리 ; 표준기저의 경우

(표기법 5.2.1) 이 절에서는 다음과 같은 notation 을 사용한다.

 \\(V = F^{n}\\) ; \\(dim V = n\\) , [\\(F^{n}\\) 의 표준기저 ] = \\(\mathcal{E} = {e_{1}, …, e_{n}}\\) .

\\(W = F^{m}\\) ; \\(dim W = m\\) , [\\(F^{m}\\) 의 표준기저 ] = \\(\mathcal{F} = {f_{1}, …, f_{m}}\\) .

\\(U = F^{r}\\) ; \\(dim U = r\\) , [\\(F^{r}\\) 의 표준기저 ] = \\(\mathcal{G} = {g_{1}, …, g_{r}}\\) .

(정의 5.2.2)\\(L \in \mathfrak{L}(F^{n} , F^{m})\\) 일 때,

\\(L(e_{1}) = \begin{pmatrix}a_{11} 



 a_{21} 



 \vdots 



 a_{m1} \end{pmatrix} , L(e_{2}) = \begin{pmatrix}a_{12} 



 a_{22} 



 \vdots 



 a_{m2} \end{pmatrix} , \cdots , L(e_{n}) = \begin{pmatrix}a_{1n} 



 a_{2n} 



 \vdots 



 a_{mn} \end{pmatrix} \\)

이라고 표기하자. (단,\\( a_{ij} \in F\\)) 이를 한 줄로 줄이면 \\(L(e_{j}) = \sum_{i = 1}^{j} a_{ij} \mathbf{f}_{i} ( j = 1,…,n)\\) 이 된다. 이때, 우리는

\\(\left[L\right]_{\mathcal{F}}^{\mathcal{E}} = \left[L\right] = (a_{ij}) = \begin{pmatrix} a_{11} & a_{12} & a_{13} & \cdots & a_{1n} 



 a_{21} & a_{22} & a_{23} & \cdots & a_{2n} 



 \vdots & \vdots & \vdots & \ddots & \vdots 



 a_{m1} & a_{m2} & a_{m3} & \cdots & a_{mn} \end{pmatrix}\\)

으로 정의하고, \\(\left[L\right]_{\mathcal{F}}^{\mathcal{E}} = \left[L\right]\\) 를 표준기저 \\(\mathcal{E}\\) 와 \\(\mathcal{F}\\) 에 관한 L 의 행렬(행렬표현) 이라고 부른다. matrix of L with respect to \\(\mathcal{E}\\) and \\(\mathcal{F}\\) 라고 부른다. 

(선형대수학의 기본정리) (정리 5.2.3) 함수 \\(\Phi_{\mathcal{F}}^{\mathcal{E}} = \Phi : \mathfrak{M}_{m,n} (F) \to \mathfrak{L}(F^{n} , F^{m})\\) 을 \\(\Phi(A) = L_{A} (A \in \mathfrak{M}_{m,n} (F))\\) 으로 정의하자. 또, 함수 \\(\Psi_{\mathcal{F}}^{\mathcal{E}} = \Psi : \mathfrak{L} (F^{n}, F^{m}) \to \mathfrak{M}_{m,n} (F)\\) 를 \\(\Psi(L) = \left[L\right]_{\mathcal{F}}^{\mathcal{E}} = \left[L\right], (L \in \mathfrak{L}(F^{n}, F^{m}))\\) 이라고 정의하면,

\\(\Phi\\) 는 isomorphism 이고 \\(\Psi\\) 는 그의 inverse map 이다.

\\(B \in \mathfrak{M}_{r,m} (F)\\) 이고 \\(A \in \mathfrak{M}_{m,n}(F)\\) 이면, \\(\Phi_{\mathcal{G}}^{\mathcal{F}} (B) \bullet \Phi_{\mathcal{F}}^{\mathcal{E}} (A) = \Phi_{\mathcal{G}}^{\mathcal{E}} (BA)\\) , 즉 \\(L_{B} \bullet L_{A} = L_{BA}\\) 가 성립한다. 또, \\(L \in \mathfrak{L}(F^{n}, F^{m})\\) 이고 \\(M \in \mathfrak{L}(F^{m} , F^{r})\\) 이면, \\(\Psi_{\mathcal{G}}^{\mathcal{F}} (M) \cdot \Psi_{\mathcal{F}}^{\mathcal{E}} (L) = \Psi_{\mathcal{G}}^{\mathcal{E}} (M \bullet L)\\) , 즉 \\(\left[M\right]_{\mathcal{G}}^{\mathcal{F}} \cdot \left[L\right] _{\mathcal{F}}^{\mathcal{E}} = \left[M \bullet L\right]_{\mathcal{G}}^{\mathcal{E}}\\) 가 성립한다.

(따름정리 5.2.5) 

모든 linear map \\(L : F^{n} \to F^{m}\\) 은 \\(L_{A}\\) 의 꼴이고, 이 때, \\(A \in \mathfrak{M}_{m,n} (F)\\) 는 유일하게 결정된다.

\\(A \in \mathfrak{M}_{m,n}(F)\\) 이면, \\(\left[L_{A}\right] = A\\) 이다.

\\(L \in \mathfrak{L}(F^{n}, F^{m})\\) 이면, \\(L_{\left[L\right]} = L\\) 이다. 따라서, \\(L(X) = \left[L\right] \cdot X , (X \in F^{n})\\) 이다.

(subsection 5.3) 기본정리 ; 일반적인 경우

(표기법 5.3.1) 이 절에서는 다음과 같은 notation 을 사용한다.

 V; \\(dim V = n\\) , [V 의 기저 ] = \\(\mathfrak{B} = {v_{1}, …, v_{n}}\\) .

W; \\(dim W = m\\) , [W 의 기저 ] = \\(\mathfrak{C} = {w_{1}, …, w_{m}}\\) .

U; \\(dim U = r\\) , [U 의 기저 ] = \\(\mathfrak{D} = {u_{1}, …, u_{r}}\\) .

위의 기저들은 모두 ordered basis 이며 모두 고정된 (fixed) 것으로 생각한다.

(정의 5.3.2) \\(L \in \mathfrak{L} (V,W)\\) 일 때

\\(\begin{cases} L(v_{1}) = a_{11}w_{1} + a_{21}w_{2} + \cdots + a_{m1}w_{m} 



 L(v_{2}) = a_{12}w_{1} + a_{22}w_{2} + \cdots + a_{m2}w_{m} 



 \vdots 



 L(v_{n}) = a_{1n}w_{1} + a_{2n}w_{2} + \cdots + a_{mn}w_{m} \end{cases} \\)

이라고 표기하자. (단,\\( a_{ij} \in F\\)). 이를 한 줄로 줄이면 \\(L(v_{j}) = \sum_{i = 1}^{m} a_{ij} w_{i} (j = 1, …, n)\\) 이 된다. 이 때, 우리는 

\\(\left[L\right]_{\mathfrak{C}}^{\mathfrak{B}} = (a_{ij}) = \begin{pmatrix} a_{11} & a_{12} & a_{13} & \cdots & a_{1n} 



 a_{21} & a_{22} & a_{23} & \cdots & a_{2n} 



 \vdots & \vdots & \vdots & \ddots & \vdots 



 a_{m1} & a_{m2} & a_{m3} & \cdots & a_{mn} \end{pmatrix}\\)

으로 정의하고, \\(\left[L\right]_{\mathfrak{C}}^{\mathfrak{B}} \in \mathfrak{M}_{m,n}(F)\\) 를 기저 \\(\mathfrak{C}\\) 와 \\(\mathfrak{B}\\) 에 관한 L 의 행렬(행렬표현) 이라고 부른다. matrix of L with respect to \\(\mathfrak{C}\\) and \\(\mathfrak{B}\\) 라고 부른다. 

(선형대수학의 기본정리) (정리 5.3.5) 함수 \\(\Phi_{\mathfrak{C}}^{\mathfrak{B}} : \mathfrak{M}_{m,n} (F) \to \mathfrak{L}( V, W )\\) 을 \\(\left[(\Phi_{\mathfrak{C}}^{\mathfrak{B}} (A))(v)\right] _{\mathfrak{C}} = A \cdot \left[v\right]_{\mathfrak{B}} (A \in \mathfrak{M}_{m,n} (F) , v \in V)\\) 으로 정의하자. 또, 함수 \\(\Psi_{\mathfrak{C}}^{\mathfrak{B}} : \mathfrak{L} (V , W ) \to \mathfrak{M}_{m,n} (F)\\) 를 \\(\Psi_{\mathfrak{C}}^{\mathfrak{B}} (L) = \left[L\right] _{\mathfrak{C}}^{\mathfrak{B}} (L \in \mathfrak{L}(F^{n}, F^{m}))\\) 이라고 정의하면,

\\(\Phi_{\mathfrak{C}}^{\mathfrak{B}}\\)  는 isomorphism 이고 \\(\Psi_{\mathfrak{C}}^{\mathfrak{B}}\\)  는 그의 inverse map 이다.

\\(B \in \mathfrak{M}_{r,m} (F)\\) 이고 \\(A \in \mathfrak{M}_{m,n}(F)\\) 이면,\\( \Phi_{\mathfrak{D}}^{\mathfrak{C}} (B) \bullet \Phi_{\mathfrak{C}}^{\mathfrak{B}} (A) = \Phi_{\mathfrak{D}}^{\mathfrak{B}} (BA)\\) 가 성립한다. 또,\\( L \in \mathfrak{L}(V, W )\\) 이고 \\(M \in \mathfrak{L}(W , U )\\) 이면, \\(\Psi_{\mathfrak{D}}^{\mathfrak{C}} (M) \cdot \Psi_{\mathfrak{C}}^{\mathfrak{B}} (L) = \Psi_{\mathfrak{D}}^{\mathfrak{B}} (M \bullet L)\\) , 즉 \\(\left[M\right]_{\mathfrak{D}}^{\mathfrak{C}} \cdot \left[L\right]_{\mathfrak{C}}^{\mathfrak{B}} = \left[M \bullet L\right] _{\mathfrak{D}}^{\mathfrak{B}}\\) 가 성립한다.

(따름정리 5.3.6) \\(L \in \mathfrak{L} (V,W)\\) 이고 \\(v \in V\\) 이면, \\(\left[L(v)\right]_{\mathfrak{C}} = \left[L\right]_{\mathfrak{C}}^{\mathfrak{B}} \cdot \left[v\right]_{\mathfrak{B}}\\) 이다.

(subsection 5.4) 기본정리의 결과와 우리의 철학

(우리의 철학 3) 행렬과 선형사상은 같은 것이다. (단, [곱셈] = [합성])

(따름정리 5.4.12) \\(A \in \mathfrak{M}_{n,n}(F)\\) 일 때, 다음 조건은 동치이다.

 \\(A\\)는 invertible matrix.

\\(L_{A}\\) :\\( F^{n} \to F^{n}\\) 은 isomorphism. 

이 때, \\((L_{A})^{-1} = L_{A^{-1}}\\) 이다.

(총정리 5.4.17) \\(A \in \mathfrak{M}_{n,n}(F)\\) 일 때, 다음 조건들은 동치이다.

\\(A\\)는 invertible matrix.

\\(A\\) 는 left inverse 를 갖는다. 즉 \\(BA = I \\)인 \\(B \in \mathfrak{M}_{n,n}(F)\\) 가 존재.

\\(A\\) 는 right inverse 를 갖는다. 즉 \\(AB = I\\) 인 \\(B \in \mathfrak{M}_{n,n}(F)\\) 가 존재.

\\(L_{A} : F^{n} \to F^{n}\\) 은 isomorphism

\\(L_{A} : F^{n} \to F^{n}\\) 은 monomorphism

\\(L_{A} : F^{n} \to F^{n}\\) 은 epimorphism

\\({\left[A\right]^{1} , …, \left[A\right]^{n}}\\) 은 \\(F^{n}\\) 의 basis.

\\({\left[A\right]^{1}, …, \left[A\right]^{n}}\\) 은 일차독립

\\(\langle \left[A\right]^{1} , …, \left[A\right]^{n} \rangle = F^{n}\\) .

\\(rk(A) = n.\\)

\\(AX = B\\) 는 unique solution 을 갖는다.

\\(AX = 0\\) 은 trivial solution 만을 갖는다.

위 조건들에 \\(A\\) 대신 \\(^{t}A\\) 를 대입한 모든 조건들.

(우리의 철학 4) 선형사상 \\(L : V \to W\\) 는\\( L_{A} : F^{n} \to F^{m}\\) 과 같은 함수이다.

(subsection 5.5) Change of Bases

(표기법 5.5.1) 이 절에서는 

 V; \\(dim V = n\\) , [V 의 기저 ] = \\(\mathfrak{B} = {v_{1}, …, v_{n}}\\), \\(\mathfrak{B}’ = {v’_{1}, …, v’_{n}}\\)

W; \\(dim W = m\\) , [W 의 기저 ] = \\(\mathfrak{C} = {w_{1}, …, w_{m}}\\) , \\(\mathfrak{C} = {w’_{1}, …, w’_{m}}\\)

U; \\(dim U = r\\) , [U 의 기저 ] = \\(\mathfrak{D} = {u_{1}, …, u_{r}}\\) .

(따름정리 5.5.2) \\(L \in \mathfrak{L} (V,W)\\) 이면, \\(\left[L\right]_{\mathfrak{C}’}^{\mathfrak{B}’} = \left[I_{W}\right]_{\mathfrak{C}’}^{\mathfrak{C}} \cdot \left[L\right]_{\mathfrak{C}}^{\mathfrak{B}} \cdot \left[I_{W}\right]_{\mathfrak{B}}^{\mathfrak{B}’}\\)

(따름정리 5.5.3) 다음이 성립한다.

\\(\left[L\right]_{\mathfrak{C}}^{\mathfrak{B’}} = \left[L\right]_{\mathfrak{C}}^{\mathfrak{B}} \cdot \left[I\right]_{\mathfrak{B}}^{\mathfrak{B}’}\\)

\\(\left[L\right]_{\mathfrak{C}’}^{\mathfrak{B}} = \left[I\right]_{\mathfrak{C}’}^{\mathfrak{C}} \cdot \left[L\right]_{\mathfrak{C}}^{\mathfrak{B}}\\)

(정의 5.5.4) V의 기저 \\(\mathfrak{B}, \mathfrak{B}’\\) 에 대해, \\(\left[I\right]_{\mathfrak{B}}^{\mathfrak{B}’}\\) 혹은 \\(\left[I\right]_{\mathfrak{B}’}^{\mathfrak{B}}\\) 을 transition matrix (한자 행렬) 라 부른다. Transition matrix 는 기저 변환 (change of bases) 의 정보를 갖고 있다.

(관찰 5.5.5) \\(\left[I\right]_{\mathfrak{B}}^{\mathfrak{B}’} \cdots \left[I\right]_{\mathfrak{B}’}^{\mathfrak{B}} = I\\) , 즉 transition matrix 는 가역이고 \\((\left[I\right]_{\mathfrak{B}’}^{\mathfrak{B}})^{-1} = \left[I\right]_{\mathfrak{B}}^{\mathfrak{B}’}\\). 역으로, 가역행렬은 항상 transition matrix 로 인식할 수 있다.

(관찰 5.5.6) \\(U \in \mathfrak{M}_{n,n} (F)\\) 가 가역행렬이고 \\(\mathfrak{B}\\) 가 V의 기저이면, 다음이 성립한다.

\\(U = \left[I\right]_{\mathfrak{B}}^{\mathfrak{B}’}\\) 인 V 의 기저 \\(\mathfrak{B}’\\) 가 존재한다.

따라서, \\(U = \left[I\right]_{\mathfrak{B}’’}^{\mathfrak{B}}\\) 인 V 의 기저 \\(\mathfrak{B}’’\\) 도 존재한다.

(관찰 5.5.7) \\(\mathfrak{B}, \mathfrak{C}\\) 가 각각 \\(F^{n}, F^{m}\\) 의 basis 이고, \\(A \in \mathfrak{M}_{m,n}(F)\\) 이면, 기본정리에 의해 \\(\left[L_{A}\right]_{\mathcal{F}}^{\mathcal{E}} = A\\) 이므로, \\(\left[L_{A}\right]_{\mathfrak{C}}^{\mathfrak{B}} = \left[I\right]_{\mathfrak{C}}^{\mathcal{F}} \cdot A \cdot \left[I\right]_{\mathcal{E}}^{\mathfrak{B}}\\) 가 성립한다.

(명제 5.5.8) \\(A,B \in \mathfrak{M}_{m,n} (F)\\) 일 때 다음은 동치이다.

\\(QAP = B\\) 인 가역행렬 \\(Q \in \mathfrak{M}_{m,m}(F)\\) 와 가역행렬 \\(P \in \mathfrak{M}_{n,n}(F)\\) 가 존재한다.

\\(\left[L_{A}\right]_{\mathfrak{C}}^{\mathfrak{B}} = B\\) 인\\( F^{n}\\) 의 basis \\(\mathfrak{B}\\) 와\\( F^{m}\\) 의 basis \\)\mathfrak{C}\\( 가 존재한다.

다음 diagram

%\begin{tikzpicture} \matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] { F^{n} & F^{m} 



F^{n} & F^{m} 



}; \path[-stealth] (m-1-1) edge node [left] {\\(\alpha_{\mathcal{E}}^{\mathfrak{B}} \\)} node [right] {\\(\approx\\)} (m-2-1)  edge node [above] {\\(L_{A}\\)} (m-1-2) (m-1-2) edge node [right] {\\(\alpha_{\mathcal{F}}^{\mathfrak{C}} \\)} node [left] {\\(\approx\\)} (m-2-2) (m-2-1) edge node [below] {\\(L_{B}\\)} (m-2-2);\end{tikzpicture}

 이 commute하는 \\(F^{n}\\) 의 basis \\(\mathfrak{B}\\) 와\\( F^{m}\\) 의 basis \\(\mathfrak{C}\\) 가 존재한다. (따라서, 이 경우에 \\(L_{A}\\) 와 \\(L_{B}\\) 는 본질적으로 같은 함수라고 말할 수 있다.)

(관찰 5.5.12) 

\\(L \in \mathfrak{L}(V,V)\\) 이고, \\(\mathfrak{B}, \mathfrak{C}\\) 가 V의 basis 이면, \\(\left[I\right]_{\mathfrak{C}}^{\mathfrak{B}} \cdot \left[L\right]_{\mathfrak{B}}^{\mathfrak{B}} \cdot \left[I\right]_{\mathfrak{B}}^{\mathfrak{C}} = \left[L\right]_{\mathfrak{C}}^{\mathfrak{C}}\\)

\\(A \in \mathfrak{M}_{n,n}(F)\\) 이고, \\(\mathfrak{B}\\) 가\\( F^{n}\\) 의 basis 이면, \\(\left[I\right]_{\mathfrak{B}}^{\mathcal{E}} \cdot A \cdot \left[I\right]_{\mathcal{E}}^{\mathfrak{B}} = \left[L_{A}\right]_{\mathfrak{B}}^{\mathfrak{B}}\\)

(정의 5.5.13) \\(A, B \in \mathfrak{M}_{n,n} (F)\\) 일 때, 만약 \\(U^{-1} A U = B\\) 인 invertible matrix \\(U \in \mathfrak{M}_{n,n} (F)\\)가 존재하면, 우리는 \\(A ~ B\\) 로 표기하고, A similar to B 라고 읽는다.

(관찰 5.5.14) 위 정의의 similarity relation 은 \\(\mathfrak{M}_{n,n} (F)\\) 의 equivalence relation 이다.

(명제 5.5.15) \\(A, B \in \mathfrak{M}_{n,n}(F)\\) 일 때, 다음은 동치이다.

\\(A ~ B\\)

\\(\left[L_{A}\right]_{\mathfrak{B}}^{\mathfrak{B}} = B\\) 인\\( F^{n}\\) 의 basis \\(\mathfrak{B}\\) 가 존재한다.

다음 diagram 

%\\(\begin{tikzpicture} \matrix (m) \left[matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em\right] { F^{n} & F^{n} 



F^{n} & F^{n} 



}; \path\left[-stealth\right] (m-1-1) edge node \left[left\right] {\\)\alpha_{\mathcal{E}}^{\mathfrak{B}} \\(} node \left[right\right] {\\)\approx\\(} (m-2-1)  edge node \left[above\right] {\\)L_{A}\\(} (m-1-2) (m-1-2) edge node \left[right\right] {\\)\alpha_{\mathcal{F}}^{\mathfrak{C}} \\(} node \left[left\right] {\\)\approx\\(} (m-2-2) (m-2-1) edge node \left[below\right] {\\)L_{B}\\(} (m-2-2);\end{tikzpicture}\\)

이 commute 하는 \\(F^{n}\\) 의 basis \\(\mathfrak{B}\\) 가 존재한다. (따라서, 이 경우에 \\(L_{A}\\) 와 \\(L_{B}\\) 가 본질적으로 같은 함수라고 말할 수 있다.)

(관찰 5.5.16) \\(A~B \in \mathfrak{M}_{n,n} (F)\\) 이면, 다음이 성립한다.

\\(dim ker L_{A} = dim ker L_{B}\\).

\\(dim im L_{A} = dim im L_{B}\\).

\\()rk(A) = rk(B)\\).

(subsection 5.6) Row-reduced echelon form

(정리 1.2.3 의 재해석)(정리 5.6.2) \\(A \in \mathfrak{M}_{m,n}(F)\\) 이면, \\(\left[L_{A}\right]_{\mathfrak{C}}^{\mathcal{E}}\\) 가 row-reduced echelon form 인 \\(F^{m}\\) 의 기저 \\(\mathfrak{C}\\) 가 존재한다. 이 때, A의 row-reduced echelon form 은 유일하게 결정된다.
