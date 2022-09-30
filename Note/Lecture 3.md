# Lecture 3

## Method of Integrating Factors

1. The most general **first order linear equation** has the form

$$
y^{\prime}=-p(t) y+g(t) \tag{1}
$$

Where $p,g$ are given functions of the independent variable $t$. 



### Example of Special Case

Solve the special case
$$
y^{\prime}=-a y+b 
$$
Where $a,b$ are constants.



To solve this equation, we may rearrange it by writing
$$
\frac{y^{\prime}}{-a y+b}=1 \Rightarrow \frac{y^{\prime}}{y-\frac{b}{a}}=-a
$$
We assume that $y \neq \frac{b}{a}$. The, we recall the chain rule for logarithms $\frac{f^{\prime}(t)}{f(t)}=(\ln |f(t)|)^{\prime}$ and notice that. $\left(y-\frac{b}{a}\right)^{\prime}=y^{\prime}$. Hence, by integration we obtain
$$
\ln \left|y-\frac{b}{a}\right|=-a t+c_1 \Rightarrow y-\frac{b}{a}=\pm e^{c_1} e^{-a t} \Rightarrow y=\frac{b}{a}+c e^{-a t} \tag{2}
$$
Where c is an arbitrary constant.



2. **Important:** in the case we assume that $y\neq \frac{b}{a}$, it is because if it equal then the left-hand side of the equatino is zero. Hence we say that $y=\frac{b}{a} \ \equiv y_{\epsilon}$ is an equilibrium. We can retrieve the equailibrium solution from the general solution (2) by seeting $c=0$.



## Integrating Factor

1. The special case is solution by direct integration, it does not work for general first order linear equation. We need to use **method of integrating factor**. 





### Example of Integrating Factor

We rewrite equation (1)
$$
y^{\prime}+p(t) y=g(t) \tag{3}
$$
Next, we multiplu both sides of the equation with a function $\mu(t)$, which is called the **integrating factor.**
$$
\mu(t) y^{\prime}(t)+\mu(t) p(t) y(t)=\mu(t) g(t) \tag{4}
$$
The next step is to find an appropriate $\mu(t)$ such that the **left-hand side of (3) is equal to the derivative of a function.** To achieve that, we recall the product rule.
$$
(f(t) h(t))^{\prime}=f^{\prime}(t) h(t)+f(t) h^{\prime}(t)
$$
We now notice that the left-hand side of (4) becomes a derivative if we set.
$$
\mu^{\prime}(t)=\mu(t) p(t)
$$
Then we can solve this equation first to know $\mu(t)$. 
$$
\begin{aligned}
\mu^{\prime}(t)=\mu(t) p(t) &\Rightarrow \frac{\mu^{\prime}(t)}{\mu(t)}=p(t) \\ &\Rightarrow \ln |\mu(t)|=\int p(t) d t+c_1 \\
&\Rightarrow \mu(t)=\pm e^{c_1} e^{\int p(t) d t} \\
&\Rightarrow \mu(t)=c e^{\int p(t) d t} \\
&\Rightarrow \mu(t)=e^{\int p(t) d t}    \quad \text{(5)}
\end{aligned}
$$
Where we picked the simplest function $\mu(t)$ with $c=1$. This is without loss of generality, since if we keep the constant $c$ and plug $\mu(t)$ into (4), we can cancel it out since it appears in all three terms of the equation. Now, with $\mu(t)$ given by (5), it follows from (4).
$$
\begin{aligned}
\mu(t) y^{\prime}(t)+\mu^{\prime}(t) y(t)=\mu(t) g(t) \\
&\Rightarrow(\mu(t) y(t))^{\prime}=\mu(t) g(t)\\
&\Rightarrow \mu(t) y(t)=\int_{t_0}^t \mu(s) g(s) d s+c \\
&\Rightarrow y(t)=\frac{1}{\mu(t)}\left(\int_{t_0}^t \mu(s) g(s) d s+c\right) .
\end{aligned}
$$
$t_0$ is some convenient lower of integration.



## Variation of Parameters

We consider again (1). We notice that if $g(t)=0$, then
$$
\begin{align}
y^{\prime}+p(t) y=0 &\Rightarrow y^{\prime}=-p(t) y \\
&\Rightarrow \frac{y^{\prime}}{y}=-p(t)\\ 
&\Rightarrow \ln |y(t)|=-\int p(t) d t+c_1 \\ 
&\Rightarrow y(t)=A e^{-\int p(t) d t}
\end{align}
$$
Where A is a constant. Next, when $g(t)$ is not everywhere zero, we look for a solution of the form. 
$$
y(t)=A(t) e^{-\int p(t) d t} \tag{6}
$$
Where A is now a function of the independent variable $t$. We substitude (6) int to (1).
$$
\begin{aligned}
&A^{\prime}(t) e^{-\int p(t) d t}-p(t) A(t) e^{-\int p(t) d t}+p(t) A(t) e^{-\int p(t) d t}=g(t) \\
&\Rightarrow A^{\prime}(t) e^{-\int p(t) d t}=g(t) \\
&\Rightarrow A^{\prime}(t)=g(t) e^{\int p(t) d t} \\
&\Rightarrow A(t)=\int_{t_0}^t g(s) e^{\int p(s) d s} d s+c
\end{aligned}
$$
The we can substitude this in to (6), then we obtain the same solution as Integrating Factor.
$$
y(t)=e^{-\int p(t) d t}\left(\int_{t_0}^t g(s) e^{\int p(s) d s} d s+c\right)
$$




## Example: Solving IVP

Solve the IVP $t y^{\prime}+(t+1) y=t$, with $y(ln2)=1$ and $t>0$. 

Solution: We write the ODE as 
$$
\begin{align}
&y^{\prime}+\frac{t+1}{t} y=1\\
&\Rightarrow y^{\prime}+\left(1+\frac{1}{t}\right) y=1
\end{align}
$$
We will use the method of the integrating factor
$$
\mu y^{\prime}+\mu\left(1+\frac{1}{t}\right) y=\mu
$$
So, we need to solve 
$$
\mu^{\prime}=\left(1+\frac{1}{t}\right) \mu \\\Rightarrow \frac{\mu^{\prime}}{\mu}=1+\frac{1}{t}\\ \Rightarrow \ln |\mu|=t+\ln t+c_1
$$
Since $t> 0$. This turn implies 
$$
\mu(t)=\pm e^{c_1} t e^t \Rightarrow \mu(t)=c t e^t \Rightarrow \mu(t)=t e^t
$$
In the final step we set $c=1$. We now recall the fundamental theorem of calculus

