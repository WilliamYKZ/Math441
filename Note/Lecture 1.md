# Math 441 Lecture 1

## ODE

1. ODE are using in physical, chemical and biological phenomena involves relations or statements of the rates at which things happen. Mathematically, we then describe these relations as equations and use derivatives to express the rates. 



2. Equations containing derivatives are called **Differential Equations**.



### Example

A spherical raindrop evaportaes at a rate proportional to its surface area. Write a differential equation for the volume of the raindrop as a function of time. 

Solution: First, we recall the volume of a sphere of radius $r$.
$$
V=\frac{4\pi}{3}r^3
$$
and the surface area of a sphere of radius $r$
$$
A=4\pi r^2
$$
Based on the statement of the problem, it holds
$$
\frac{dV}{dt}=-k4\pi r^2
$$
This equation is correct, but it does not provide the final answer. we need to express $r$ in terms of $V$. In this way, we will have time $t$ as the independent variable and the volume $V=V(t)$ as the dependent variable.
$$
r^3=\frac{3V}{4\pi}\Rightarrow r=(\frac{3V}{4\pi})^{\frac{1}{3}}
$$
Which if we plug into the previous equation yields


$$
\frac{d V}{d t}=-k 4 \pi\left(\frac{3 V}{4 \pi}\right)^{\frac{2}{3}}
$$
We may simpilfy this ODE, by combining all constants into one 
$$
\frac{dV}{dt}=-kV^{\frac{2}{3}}
$$
Since differentiation and integration are inverse processes, we may recall some 

tricks from integration to help us solve ODEs. **separation of variables** is a good methods to solve ODEs. Specifically, we sepaeate the unknown variable $V$ and its derivative from the independent variable $t$ and any constants that are assumed to be known. In the previous problem, we proceed as follows. We may express the derivative as $V^\prime =\frac{dV}{dt}$. Then
$$
V^{\prime}=-\kappa V^{\frac{2}{3}} \Rightarrow \frac{V^{\prime}}{V^{\frac{2}{3}}}=-\kappa
$$
Now, we may use the chain rule
$$
\frac{d}{d t} f(g(t)) \equiv(f(g(t)))^{\prime}=f^{\prime}\left(g(t) g^{\prime}(t)\right.
$$
to integrate the left hand side. Then chain rule for powers of functions become. 
$$
\frac{d}{d t}\left(V^{a}(t)\right)=a V^{a-1}(t) V^{\prime}(t) \Rightarrow \frac{V^{\prime}}{V^{1-a}}=\frac{1}{a} \frac{d}{d t}\left(V^{a}(t)\right)
$$
with $1-a = \frac{2}{3}\Rightarrow a = \frac{1}{3}$. Hence 
$$
3 \frac{d}{d t} V^{\frac{1}{3}}(t)=\frac{V^{\prime}}{V^{\frac{2}{3}}}=-\kappa \Rightarrow \frac{d}{d t} V^{\frac{1}{3}}(t)=-\frac{\kappa}{3} \Rightarrow V^{\frac{1}{3}}(t)=-\frac{\kappa}{3} t+c
$$
Where $c$ is a constant of integration. After some algebraic manipulations we obtain.
$$
V(t)=\left(c-\frac{\kappa t}{3}\right)^{3}
$$


## Initial Value Problems 

1. Problem with initial conditions are called Initial Value Problems (IVP). For instance, in the previous problem, they could have given us the volume of the drop at time $t=0,V(0)=V_0$. Then, it would be 

$$
V(0)=c^{3}=V_{0} \Rightarrow V(t)=\left(V_{0}^{\frac{1}{3}}-\frac{\kappa t}{3}\right)^{3}
$$



## More Example 

