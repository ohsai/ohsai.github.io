---
layout: post
title : (Linear Algebra) Vector space 벡터 공간
date : 2018-01-19 13:51:04 +0900
---
(Section 2) 벡터공간

(subsection 2.1.) Vector Space

(표기법 2.1.1) \\(F^{n} = \mathfrak{M}_{n,1}(F)\\).


(정의 2.1.2) F가 위와 같고, 집합 V에 덧셈과 상수곱이 주어져 있을 때, 다음 연산규칙들을 만족하면 V를 F 위의 벡터공간 (vector space over F, 혹은 F-vector space) 라 부른다. 또, V의 원소들을 vector라 부르고, F의 원소를 scalar라 부른다.


\\(u,v,w \in V\\) 이면, \\((u+v) +w = u + (v + w)\\) (덧셈의 결합법칙)


\\(v, w \in V\\) 이면 , \\(v + w = w + v\\) (덧셈의 교환법칙)


(모든 \\(v \in V\\) 에 대하여 \\( v + 0 = v\\)) 인 \\(0 \in V\\) 존재 (덧셈의 항등원)


\\(v \in V \\)이면, \\(v + (-v) = 0\\) 인 \\(-v \in V\\) 존재. (덧셈의 역원)


\\(a,b \in F\\) ,\\( v \in V\\) 이면, \\((a + b) v = av + bv\\) (분배법칙)


\\(a \in F\\), \\(v, w \in V\\) 이면, \\(a(v+w) = av + aw\\) (분배법칙)


\\(a, b \in F\\), \\(v \in V\\) 이면, \\(a(bv) = (ab)v\\)


\\(v \in V\\) 이면, \\(1v = v\\)


(관찰 2.1.3) 


vector space V 의 덧셈의 항등원 \\(0 \in V\\) 는 유일하다.


\\(v \in V\\) 이면, v의 덧셈의 역원 \\(-v \in V\\) 는 유일하다.


(표기법 2.1.4) 유일성이 보장된 \\(0 \in W\\) 를 the zero vector 라 부른다. \\(v \in w\\) 일 때, \\(v -w = v + (-w)\\) 로 쓴다.


(Cancellation law) (관찰 2.1.5) \\(u,v,w \in V\\) 이면, 다음 \\( \left[u + v = u + w \right] \implies \left[ v = w \right] \\) 이 성립한다. 즉, \\(u + v = u + w\\) 양 변에서 u 를 cancel 할 수 있다.


(관찰 2.1.7) \\(v \in V\\) 이고 \\(a \in F\\) 이면,


\\(0v = 0\\).


\\(a0 = 0 \in V\\).


\\(-v = (-1) v\\).


\\(-(av) = (-a) v\\).


\\(-(av) = a(-v)\\).


(subsection 2.2) Subspace 


(정의 2.2.2) W가 F-vector space V 의 subset 일 때 (즉, \\(W \subseteq V\\) 일 때,) V로부터 물려받은 덧셈과 상수곱에 대하여 ,W 자신이 F-vector space 가 되면, 우리는 W를 V의 F-subspace (부분공간, 혹은 간단히 subspace) 라 부르고, \\)W \le V\\) 로 표기한다.


(관찰 2.2.3) F-vector space V 의 non-empty subset W 가 V의 subspace 일 필요충분조건은 다음과 같다. 즉, W가 덧셈과 상수곱에 대해 닫혀있으면 , V의 subspace 가 된다.


\\(w_{1} , w_{2} \in W\\) 이면, \\(w_{1} + w_{2} \in W\\).


\\(w \in W\\) 이고 \\(a \in F\\) 이면, \\(aw \in W\\).


(관찰 2.2.5) \\(U \le W\\) 이고 \\(W \le V\\) 이면, \\(U \le V\\) 이다. (subspace의 subspace는 subspace이다.)


(표기법 2.2.6) \\(W_{1} , \cdots, W_{k} \subseteq U\\) 일 때, \\(\sum_{i = 1}^{k} W_{i} = W_{1} + \cdots + W_{k} = \lbrace w_{1} + \cdots + w_{k} \| w_{1} \in W_{1}, \cdots, w_{k} \in W_{k} \rbrace \\) 로 표기하고 \\(W_{1} \cdots , W_{k}\\) 의 합(sum)이라고 부른다.


(subspace 2.4) Isomorphism


(정의 2.4.1) V와 V’ 이 F-vector space 이고, 다음 조건


\\(\phi(v_{1} + v_{2}) = \phi(v_{1}) + \phi(v_{2}) , (v_{1}, v_{2} \in V) \\)


\\(\phi(av) = a \phi(v) (v \in V, a \in F)\\) 


을 만족하는 bijection \\(\phi: V \to V’\\) 이 존재하면, 우리는 F-vector space V 와 V’ 이 isomorphic 하다 말하고, \\(V \approx V’ \\)혹은  
\begin{tikzpicture}
\matrix (m) [matrix of math nodes,row sep=3em,column sep=4em,minimum width=2em] 
{V &V’};\path[-stealth](m-1-1) edge node [above] {\\)\phi\\(} node [below]{\\)\approx\\)} (m-1-2);
\end{tikzpicture}  
로 표기한다. 이 때, $$\phi$$ 를 (F-vector space) isomorphism (from V onto V’) 이라고 부른다.  
(관찰 2.4.2) $$\phi : V \to W$$ 가 isomorphism 이면, $$\phi(0) = 0$$ 이고, 모든 $$v \in V$$에 대해 $$\phi(-v) = -\phi(v)$$ 이다.  
(관찰 2.4.4) 위 (정의 2.4.1) 의 relation $$\approx$$ 는 equivalence relation 이다.  
