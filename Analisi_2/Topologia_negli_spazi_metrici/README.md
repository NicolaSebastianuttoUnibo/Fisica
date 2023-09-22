# Topologia negli spazi metrici

## Lezione1

Topologia negli spazi metrici
Topologia $\to$aperto/chiuso
spazi metrici $\to$distanza fra punti nell'insieme X


**Def:(spazio metrico)**
$(X,d)$ con d: $X\times X \Rightarrow [0,\infty ]$

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
1/d_{ij} & \quad \text{when $d_{ij} \leq 160$}\\ 
0 & \quad \text{otherwise}
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
 |x_i-y_i| \le \underset{\underset{1 \leq i \leq n}{\max |x_i-z_i|}}{\underline{|x_i-z_i|}}+ \underset{\underset{1 \leq j \leq n}{\max |z_j-y_j|}}{\underline{|z_i-y_i|}}

$|x_i-y_i| \le \underset{\underset{a}{b}}{b}$


 $\forall i |x_i-y_i| \le d_{\infty} (\underline{x},\underline{z})+d_{\infty} (\underline{z},\underline{y})$

$d_{\infty} (\underline{x},\underline{y})=\underset{1  \le i \le n}{\max}|x_i-y_i|\le d_{\infty}(\underline{x},\underline{z})+d_{\infty}(\underline{z},\underline{y})$