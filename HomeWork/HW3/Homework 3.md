# Homework 3

## Question 1

$$
\begin{align}
x y^{\prime}(x)=2 y(x)\\
&\Rightarrow y^\prime = \frac{2y}{x}\\
&\Rightarrow y^\prime -\frac{2}{x}y = 0\\
\end{align}
$$

Consider $\mu(x) = e^{-1\int\frac{2}{x}dx}=\frac{1}{x^2}$. and multiply $\mu(x)$ on both side:
$$
\frac{1}{x^2}y^\prime -\frac{2}{x^3}y = 0 \Rightarrow (\frac{1}{x^2}y)^\prime = 0\Rightarrow \frac{1}{x^2}y = C\Rightarrow y=Cx^2
$$
From the question, it give us $y(0)=0$. Thus $0\cdot C = 0$, and $C$ can be any number. 



It is not violate the existence and uniqueness theorem. By $y^\prime =\frac{2y}{x}$ and $\frac{\partial f(x, y)}{\partial y}=\frac{2}{x}$ they are all continuous everywhere when $x\neq 0 $. Thus the existence and uniqueness theorem will noe violate when $x=0$, which is the question initial condition. Thus we cannot know if tere are unique solution or have a solution by the theorem.  





## Question 2

$$
\begin{align}
\frac{d y}{d x}=3 y^{\frac{2}{3}}\\
&\Rightarrow y^\prime = 3y^\frac{2}{3}\\
&\Rightarrow  y^{\prime}+0 y=3 \cdot y^\frac{2}{3}

\end{align}
$$

Consider $\mu(x) = y^\frac{1}{3}$, we can know that the equation is a Bernoulli equation with $n=\frac{2}{3}$. and we can get
$$
3\mu^2\cdot \mu^\prime =3\cdot \mu^2
$$

- Consider $\mu \neq0$, Which we have $y\neq 0$ and $\mu^\prime = 1$
  $$
  y(x)=\mu(x)^3=(x+C)^3, \quad y(x)\neq 0
  $$

- The question give us $y(0)=0$,
  $$
  y(0)=(0+C)^3 = 0
  $$
  Thus we can know $C=0$. Thus $y(x)=x^3$, $y(x)\neq 0$

When $y(x)=0, y^\prime =0, 3y^\frac{2}{3}=3\cdot 0^\frac{2}{3}=0$. and we can get $y(x) = x^3$ and $y(x)=0$. 



Since $y^{\prime}=f(x, y)=3 y^{2 / 3}$ is continuous everywhere, and $\frac{\partial f}{\partial y}=\frac{2}{\sqrt[3]{y}}$ is continuous everywhere when $y\neq 0$. The existence and uniqueness theorem, for $y>0$ and $y<0$. and it did not contradict because the initial value the question give us $(0,0)$ is not satisfy the assumption. 



## Question 3

$$
\begin{align}
2 x y y^{\prime}=4 x^2+3 y^2\\
&\Rightarrow y^{\prime}=\frac{4 x^2+3 y^2}{2 x y}\\
&\Rightarrow  y^{\prime}-\frac{3y}{2 x} = 2x\cdot y^{-1}

\end{align}
$$

We can know the $n=-1$, Consider $\mu(x) = y^2$.and $y=\pm \sqrt v$

- Consider $y=\sqrt v$
  $$
  \begin{align}
  y^{\prime}=\frac{1}{2} \cdot \mu^{-\frac{1}{2}} \cdot \mu^{\prime}\\
  \frac{\mu^{-\frac{1}{2}} \cdot \mu^{\prime}}{2}-\frac{3 \mu^{\frac{1}{2}}}{2 x}=2 x \mu^{-\frac{1}{2}}\\
  \mu^{\prime}-\frac{3}{x} \mu=4 x
  
  \end{align}
  $$
  Consider $u(x)=e^{-\int \frac{3}{x} d x}=e^{-3 \ln |x|} = |x|^{-3}$.Then we can know $\left(x^{3}\mu\right)^{\prime}=4 x^{-2}$ when $x>0$. 

  Then we can know $x^{-3} \mu=4 \int x^{-2} d x=\frac{-4}{x}+C$. 

  At last we can get $y(x)=\pm x\sqrt{Cx-4}$ where C is arbitrary constant number.





## Question 4

$$
\begin{align}
x y^{\prime}+6 y=3 x y^{\frac{3}{3}}\\
&\Rightarrow y^{\prime}+\frac{6}{x} y=3 y^\frac{4}{3}
\end{align}
$$

We can know $n=\frac{4}{3}$. Consider $\mu(x) = y^\frac{-1}{3}$ $y\neq 0$. and then we can know $y^{\prime}=-3 \mu^{-4} \cdot \mu^\prime $. 
$$
-3 \mu^{-4} \cdot \mu^\prime+\frac{6}{x} \cdot \mu^{-3}=3 \cdot \mu^{-4}\\
\Rightarrow \mu^{\prime}-\frac{2}{x}\mu = -1
$$
Consider $u(x)=e^{-\int \frac{2}{x}dx}=|x|^{-2}$, suppose $x>0$ we can know $u(x)=x^{-2}$. Multiplying $u(x)$ on both side.
$$
\left(x^{-2} \cdot \mu\right)^{\prime}=-x^{-2}\\
x^{-2} \cdot \mu=-\int x^{-2} d x=\frac{1}{x}+C\\
\mu=\left(\frac{1}{x}+c\right) x^2=x+c x^2 .
$$
Then we can know $y(x)=\left(x+C x^2\right)^{-3} = \frac{1}{x^3(C x+1)^3}$. 

Then when $y(x)=0$, $y^\prime(x) =0$. $x y^{\prime}+6 y^2=3 x y^{\frac{4}{3}}=0$. Thus we can get $y(x)=\frac{1}{x^3(C x+1)^3}$ and $y(x)=0$. 





## Question 5

(a) $V(t)=V_0+(2-3) t=60-t$, when $(0 \leq t \leqslant 60)$. Thus the volume of fluid in the tank after $t \ min$ will be $60-t$ gallen. 



