# Topologia negli spazi metrici

## Lezione1 ()()

Topologia negli spazi metrici
Topologia $\to$aperto/chiuso
spazi metrici $\to$distanza fra punti nell'insieme X

* Def:(spazio metrico) 
$(X,d) con d:X\times X \Rightarrow [0,\infty [$

con le seguenti proprietà
$\forall x,y,z \in \mathbb{R}$
1. $d(x,y)=0 \Leftrightarrow x=y$
2. $d(x,y)=d(y,x)$
3. $d(x,y) \le d(x,z)+d(z,x)$

** Modello
$X=\mathbb{R}; d(x,y)=|x-y|; \mathbb{R} spazio euclideo$
1. $|x-y|=0 \Leftrightarrow x-y=0 \Leftrightarrow x=y$
2. $|x-y|=|y-x|$
3. $|x-y|=|x-z+z-y| \le|x-z|+|z-y|$

* Esempi
$
\begin{enumerate}
\item X= \mathbb{R}^n=\{\underline{x}=(x_1,...,x_n):x_i \in \mathbb{R} \forall i=1,...,n\};
\item \displaystyle a) d_1 (\underline{x},\underline{y}=\sum_{i=1}^{n}|x_i-y_i|) 
\item \displaystyle b) d_2 (\underline{x},\underline{y}=\left(\sum_{i=1}^{n}(x_i-y_i)^2\right)^{1/2}) 
\item \displaystyle c) d_p (\underline{x},\underline{y}=\left(\sum_{i=1}^{n}(x_i-y_i)^p\right)^{1/p}) 
\item \displaystyle d) d_{\infty} (\underline{x},\underline{y}=\left(\sum_{i=1}^{n}(x_i-y_i)^p\right)^{1/p}) 

\end{enumerate}

$

