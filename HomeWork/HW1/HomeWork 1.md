# HomeWork 1

## Question 1

From the question we can know there is a tangent line to the graph $g$ at the point $(x,y)$ intersects the $x-axis$ at the point $(\frac{x}{3},0)$. Thus we can know 
$$
\begin{align}
g^\prime(x) &= \frac{-y}{\frac{x}{3}-x}\\
&= \frac{-y}{\frac{x-3x}{3}}\\
& = \frac{3y}{2x}
\end{align}
$$
Thus we find the differential equation $\frac{dy}{dx}=\frac{3y}{2x}$ will have a solution $g$.





## Question 2

First we can simplfy the equation
$$
\begin{align}
y^\prime +2xy^2=0 \Rightarrow 
\frac{dy}{dx}&=-2xy^2\\
\frac{dy}{y^2} &= -2xdx
\end{align}
$$
Now we can integrate both sides.
$$
\begin{align}
\int \frac{dy}{y^2}&=\int -2xdx\\
 -\frac{1}{y}&=-x^2+c\\
 \frac{1}{y} &= x^2+c \tag{1}
\end{align}
$$
Which $c$ is a constant. and it also why when we do equation (1), we didn't add minus sign on $c$.

Finally, we can write the function.
$$
y=\frac{1}{x^2+c}
$$





## Question 3

(a)

The ODE is a nonlinear equation. We can first simplfy the equation. 
$$
e^yy^\prime = 1 \\
e^yy^\prime -1 =0
$$
We cannot find a way to let equation rewrite to linear different equation formula $a(x)y^\prime + b(x)y$. Thus it is a nonlinear equation.

(b)

First we focus on $y=ln(x+C)$. and that its derivative.
$$
\frac{dy}{dx}=\frac{1}{x+C}
$$
Then plug in to equation. 
$$
e^yy^\prime =e^{ln(x+C)}\cdot \frac{1}{x+C} = |x+C|\cdot \frac{1}{x+C}=1
$$
Thus we can know $y=ln(x+C)$ is the solution of equation when $x>-C$



(c)
$$
y(0)=0 \Leftrightarrow ln(0+C) = 0\Leftrightarrow ln(C) = 0
$$
Clearly, we can know $C=1$





## Question 4

$$
\begin{align}
2 x y^{\prime}+y &=10 \sqrt{x}  \tag{1}  \\
y^{\prime}+\frac{y}{2 x}&=10 \frac{\sqrt{x}}{2 x} \tag{2}\\
y^{\prime}+\frac{y}{2 x}&= \frac{5}{\sqrt{x}} \\
\end{align}
$$

We divided $2x$ both side of equation (1), and simplify the equation (2). Since the equation is the first order linear equation so we condifer the form $y^\prime = -p(t)y+g(t)$
$$
p(t)=\frac{1}{2x} \quad and \quad g(t)=\frac{5}{\sqrt{x}}
$$
Now we can integrate the differential equation. 
$$
e^{\int p(x)dx} = e^{\int \frac{1}{2x}dx} = e^{2ln(x)}=e^{ln(\sqrt{x})}=\sqrt{x}
$$
Now the different equation will be 
$$
y\sqrt{x}=\int \frac{5}{\sqrt{x}}\sqrt{x}dx+c\\
y\sqrt{x}=5x+c\\
y = 5\sqrt{x}+\frac{c}{\sqrt{x}}
$$
Since the question give us $y(1)=2$. we can slove $c=-3$. then the different equation will be. 
$$
y = 5\sqrt{x}+\frac{-3}{\sqrt{x}}
$$

## Question 5

First focus on the equation. 
$$
\begin{aligned}
&2 x \frac{d y}{d x}-y=2 x \cos x \\
&\frac{d y}{d x}-\frac{y}{2 x}=\cos x
\end{aligned}
$$
Since, it is a linear different  equation. we can use the formula of the linear different equation.
$$
p(k)=-\frac{1}{2x} \ and \ q(x) = cos(x)
$$
So we can get 
$$
e^{\int p(d)dx}=e^{-\frac{1}{2}lnx}=e^{lnx^{-\frac{1}{2}}}=\frac{1}{\sqrt{x}}
$$
So we can get 
$$
y\cdot \frac{1}{\sqrt x}=\int \frac{1}{\sqrt x}\cdot cosx dx +C\\
y = \sqrt x \cdot (\int \frac{1}{\sqrt x}\cdot cosx dx +C)
$$
