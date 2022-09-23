# Lecture 2

## Ordinary and Partial Differential Equation

1. The unknown function $y$ depends on a single independent variable. In this case, only ordinary derivatives appear in the differential equation which is an ODE.

$$
\frac{dy}{dt}=3t^2y
$$



2. When the unknown function $y$ depends on more than one independent variables, partial derivatives appear in the differential equation which is a PDE, such as

$$
u_{tt}=c^2u_{xx}
$$



## System of Differential Equation

1. A system is a collection of ODEs or PDEs. the **dimension** of the system is equal to the number of equation there, which is equal to the number of unknown function. 

$$
\begin{aligned}
&S^{\prime}=-\beta S I \\
&I^{\prime}=\beta S I-\gamma I \\
&R^{\prime}=\gamma I
\end{aligned}
$$



## Order

1. The **order** of a differential equation is the order of the highest derivative that appears in the equation. 

### Example1

$$
m u^{\prime \prime}(t)+\gamma u^{\prime}(t)+k u(t)=0
$$

is a second-order equation. 



2. More importantly we can change hight order ODE to a system ODE with 1 order ODE.

### Example2

Keep the equation before, we need to set $u_1=u,u_2=u^\prime$. which implies
$$
u_1^{\prime}=u^{\prime}=u_2, \quad \text { and } m u_2^{\prime}+\gamma u_2+k u_1=0
$$
and by rearranging the second equation we obtain.
$$
\begin{aligned}
u_1^{\prime} &=u_2 \\
u_2^{\prime} &=-\frac{k}{m} u_1-\frac{\gamma}{m} u_2
\end{aligned}
$$




## Linear and Nonlinear Equation

1. An ODE of the form 

$$
F\left(t, y, \ldots y^{(n)}\right)=0
$$

is said to be **linear** if $F$ is a linear function of the variables $y, y^{\prime}, \ldots y^{(n)}$. Hence, the general linear ODE of order $n$ is.
$$
a_n(t) y^{(n)}+a_{n-1}(t) y^{(n-1)}+\ldots+a_1(t) y^{\prime}+a_0(t) y=g(t)
$$


2. An equation that is not of the form is a **nonlinear** equation. The so-called equation of **logistic growth**. 

$$
y^{\prime}=r y\left(1-\frac{y}{K}\right)
$$



## Existence, Uniqueness, Continuous Dependence on Initial Conditions

1. Not all ODEs have a solution. We are interested in the conditions on $f$ in $\dagger$ that ensure existence of solutions. For those ODEs that have a solution, this solution may not be unique. This is undesirable when the problem models a physical process. Finally, we are interested to know what happens if we perturb slightly the initial conditions of the ODE. Will the solution change dramatically? This is the question of continuous dependence on initial conditions.

