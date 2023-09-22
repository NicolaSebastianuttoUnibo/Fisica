# Topologia negli spazi metrici

## Lezione 1

Topologia negli spazi metrici
Topologia $\to$aperto/chiuso
spazi metrici $\to$distanza fra punti nell'insieme X

### Spazio metrico

,**Def:(spazio metrico)**
$(X,d)$ con d: $X\times X \rightarrow [0,\infty [$

con le seguenti proprietà
$\forall x,y,z \in \mathbb{R}$
1. $d(x,y)=0 \Leftrightarrow x=y$
2. $d(x,y)=d(y,x)$
3. $d(x,y) \le d(x,z)+d(z,x)$

**Modello** 
$X=\mathbb{R}; d(x,y)=|x-y|; \mathbb{R}$ spazio euclideo
1. $|x-y|=0 \Leftrightarrow x-y=0 \Leftrightarrow x=y$
2. $|x-y|=|y-x|$
3. $|x-y|=|x-z+z-y| \le|x-z|+|z-y|$

**Esempi**


$X= \mathbb{R}^n=\{\underline{x}=(x_1,...,x_n):x_i \in \mathbb{R} \forall i=1,...,n\};$

(a) $$\displaystyle  d_1 (\underline{x},\underline{y}=\sum_{i=1}^{n}|x_i-y_i|) $$

(b) $$\displaystyle  d_2 (\underline{x},\underline{y}=\left(\sum_{i=1}^{n}(x_i-y_i)^2\right)^{1/2})$$ 

(c) $$\displaystyle  d_p (\underline{x},\underline{y}=\left(\sum_{i=1}^{n}(x_i-y_i)^p\right)^{1/p}) $$

(d) $$\displaystyle  d_{\infty} (\underline{x},\underline{y})= \underset{1 \leq i \leq n}{\max}$$

(e) 

$$
S(\underline{x},\underline{y})=
\begin{cases}
0 & \underline{x}=\underline{y}\\ 
1 & \underline{x}\neq \underline{y}
\end{cases}
$$




 Ora verifichiamo gli spazi mettrici a,d,e

 **proprietà (1)**

(a) $\sum_ |x_i-y_i|=0 |\Leftrightarrow |x_i-y_i|=0\forall i=1,...,n \Leftrightarrow x_i=y_iforall i=1,...,n$

(d) $\underset{1 \leq i \leq n}{\max}|x_i-y_i|=0 \Leftrightarrow  |x_j-y_j| \forall j \Leftrightarrow x_y=y_j \forall j=1,...,n$

(e)
per definizione

 **proprietà (2)**

 $d(\underline{x},\underline{y})=d(\underline{y},\underline{x})$

 (a) (d) sege dal fatto che vale  in $\mathbb{R}$
 (e) case by case

 **proprietà (3)**

 (a)

 $d(\underline{x},\underline{y}) \le d(\underline{x},\underline{z})+d(\underline{z},\underline{y})$

 $\sum_ |x_i-y_i|=\sum_ |x_i-z_i+z_i-y_i| \le \sum_ (|x_i-z_i|+|z_i-y_i|)\le sum_ |x_i-z_i|+sum_ |z_i-y_i|$

 (d) 

$|x_i-y_i| \le \underset{\underset{1 \leq i \leq n}{\max |x_i-z_i|}}{\underline{|x_i-z_i|}}+\underset{\underset{1 \leq j \leq n}{\max |z_j-y_j|}}{\underline{|z_i-y_i|}}$


 $\forall i \quad |x_i-y_i| \le d_{\infty} (\underline{x},\underline{z})+d_{\infty} (\underline{z},\underline{y})$

$d_{\infty} (\underline{x},\underline{y})=\underset{1  \le i \le n}{\max}|x_i-y_i|\le d_{\infty}(\underline{x},\underline{z})+d_{\infty}(\underline{z},\underline{y})$ 

(e)
case by case
$\delta( \underline{x},\underline{y}) \le \delta(\underline{x},\underline{z})+(\delta \underline{z},\underline{y})$

case $ \underline{x}= \underline{y}= \underline{z}$

$0 \le 0+0$

case $ \underline{x}= \underline{y}\neq \underline{z}$

$0 \le 1+1$

case $ \underline{x}= \underline{z}\neq \underline{y}$

$1 \le 0+1$

case $ \underline{y}= \underline{z}\neq \underline{x}$

$1 \le 1+0$

case $ \underline{x}\neq \underline{y}\neq \underline{z}$

$1 \le 1+1$

**Altro esempio**

$x={f:[a,b] \rightarrow \mathbb{R} \text{continua} } \quad f,g \in X$

 - $d_1(f,g)=\int_{a}^{b}|f(x)-g(x)|dx$

  verifichiamo che sia uno spazio metrico

 1. $0=d_1(f,g)=\int_{a}^{b}|f(x)-g(x)|dx \Rightarrow f(x)=g(x) \forall x \in  [a,b]$

 suppponiamo per aassurdo che $f(\overline{x}) \neq g(\overline{x}) per un qualche \overline{x} \in [a,b]$

 per il 'Teorema di permanenza del segno' in un intorno di $\overline{x}$ contenuto in $[a,b]$

 $|f(x)-g(x)| \ge \frac{d|f(\overline{x})-g(\overline{x})|}{2}$

 questo rende impossibile il fatto che l'integrale sia nullo

 2. ovvia $|f(x)-g(x)|=|g(x)-f(x)|$

 3. $\int_{a}^{b}|f(x)-g(x)|dx=\int_{a}^{b}|f(x)+h(x)-h(x)-g(x)|dx \le \int_{a}^{b}(|f(x)-h(x)|+|h(x)-g(x)|)dx \le \int_{a}^{b}|f(x)-h(x)|dx+\int_{a}^{b}|h(x)-g(x)|dx$

 - $d_2(f,g)=\left(\int_{a}^{b}|f(x)-g(x)|^2dx\right)^{1/2}$

 - $d_{\infty}(f,g)=\underset{a \le x  \le b}{\max} |f(x)-g(x)|$

### Topologia

**Def:(topologia)**
  $X$ insieme $\tau$ una famiglia di sottoinsieme di $X$, la coppia $(X,\tau)$ è una topologia se ha le seguenti proprietà:

  1. $X,\varnothing \in \tau$
  2. $A_{\alpha},A_{\beta} \in \tau \forall \alpha, \beta \Rightarrow A_{\alpha}\cup A_{\beta} \in \tau$
  3. $A_{\alpha},A_{\beta} \in \tau \forall \alpha, \beta \Rightarrow A_{\alpha}\cap A_{\beta} \in \tau$

In tal caso gli elemnti $\tau$ si chiamano aperti (rispetto alla topologia $(X,\tau )$)

  Per associare una topologia ad uno spazio  metrico  **prima** dobbiamo definire l'inotrno circolare aperto

**Def:(inotrno circolare aperto)**

Siano $x_0 \in X \quad r>0$, chiamo  intorno circolare aperto di $x_0$ di raggio $r$

$B_{r_0}(x)={x \in X : d(x,x_0)<r>}$

Esempi:
- 
prendiamo lo spazio metrico $d_2$; $X=\mathbb{R}^2$; $\underline{x}=(x_1,x_2)$; $\underline{x_0}=(x_1^0,x_2^0)$

$\mathbb{B}_{x_0}(r)={x \in \mathbb{R}^2:(x_1-x_2^0)^2+(x_2-x_1^0)^2<r^2>}$

immaginati una sfera centrato in $(x,y)$ di raggio $r$ SENZA CONTORNO

- 
prendiamo lo spazio metrico $d_1\text{;}\quad X=\mathbb{R}^2\text{;}\quad \underline{x}=(0,0)\text{;}\quad \underline{x_0}=(x_1,x_2)$


$d(\underline{x},0)=|x_1|+|x_2|<r$
immaginati un rombo di raggio di $2r$ centrato in origine

- 
prendiamo lo spazio metrico $d_{\infty}=\max {|x_1|,|x_2|}$; $X=\mathbb{R}^2; $

immaginati un quadrato di lato $2r$ pieno

**Def:(Insieme aperrto)**
$A \in X \text{è aperto se }\forall x \in A  \exists x>0 t.c. B_r(x) \subseteq A$

**Proposizione:** Ogni intorno circolare aperto è un aperto in $(X,d)$

$y \in B_r(x_0) \quad d(x_0,y)=\delta<x \overline{r} =\min {\delta, r-\delta}$

$B_{\overline{r}}(y) \quad d(z_0,z) \le d(x_0,y)+d(y,z) \le \delta + \overline{r} \le&
 $$\begin{cases}
\delta +r -\delta-r-r \quad \overline{r}=r-\delta
r \quad  \overline{r}=\delta \le frac{\delta}{2}
\end{cases}

$$
