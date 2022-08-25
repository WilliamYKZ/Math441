# Chapter 1

## Some Basic Mathematical Models; Direction Firlds

1. Equation containing derivatices are **differential equations**. And a differential equation that describes some physical process is often called a **mathematical model** of the process, and many such models are discussed throughout this book. 

### Example 1 : A Falling Object

Description: we use $t$ to denote time. $v$ represent the velocity of the falling object. Since the velocity will presumably change with time, so we think of $v$ as a function of $t$. We using Newton's second law for the motion of object. 
$$
F=ma \tag{1}\\
$$
$a$ represent acceleration, and $a$ is related to $v$ by $a = \frac{dv}{dt}$, so we can rewrite equation (1)
$$
F=m\frac{dv}{dt} \tag{2}
$$
Next consider the forces that act on the object as it falls. Gravity exerts a force equal to the weight of the object, or $mg$. There is also a force dut to air resistance, or drag. the drag force has the magnitude $\gamma$ where $\gamma$ is a contant called the drag coefficient. Then we can write a new equation.
$$
F = mg-\gamma v \tag{3}
$$
![](https://github.com/WilliamYKZ/Picture/raw/main/Picture/Screen%20Shot%202022-08-25%20at%207.51.11%20AM.png)

Let us assume $m=10kg$ and $\gamma = 2kg/s$
$$
\frac{d v}{d t}=9.8-\frac{v}{5}
$$




## Solution of Some Differential Equations

### Example2:

Consider the eqation 
$$
\frac{dp}{dt}=0.5p-450 \tag{1}
$$
which describes the interaction of certain populations of field mice and owls. Find solution of this equation

Solution:

To solve equation, we need to find functions $p(t)$, which subsituted into the equation, reduce it to an obvious identity, Here is one way to proceed.
$$
\begin{align}
\frac{dp}{dt} &= \frac{p-900}{2} \tag{2}\\

\end{align}
$$
or if $p\neq 900$
$$
\frac{d p / d t}{p-900}=\frac{1}{2} \tag{3}
$$
By the chain rule the left-hand side of equation (3) is the derivative of $ln|p-900|$ with respect to $t$, so we have. 
$$
\frac{d}{d t} \ln |p-900|=\frac{1}{2} \tag{4}
$$
Then, by integrating both sides of equation (7), we obtain.
$$
\ln |p-900|=\frac{t}{2}+C \tag{5}
$$
Where $C$ is an arbitrary constant of integration. Therefore, by taking the exponential of both sides of equation (5), we find that 
$$
|p-900|=e^{t / 2+C}=e^{C} e^{t / 2}\\
p=900+c e^{t / 2}
$$
Frequently, we want to focus our attention on a single member of the infinite family of solutions by specifying the value of the arbitrary constant. For example, to determine the constant $c$ in equation, we could require that the population have a given value at a certain time, such as value 850 at time $t=0$. The we can use that to get $c=-50$
$$
p = 900-50e^{\frac{t}{2}}
$$


1. The additional condition that we used to determine $c$ is an example of an **initial condition.** The differential equation together with the initial condition forms an **initial value problem**. 





## Classification of Differential Equations

1. Only ordinary derivatives appear in the differential equation, and it is said to be **ordinary differential equation**. the derivatives are partial derivatives, and the equation is called a **partial differential equation**. 

   

2. Another classification of differential equations depends on the number of unknown functions that are involved. if there are two or more unknown functions, then a sysatem of differential equation is required. 
   $$
   \begin{aligned}
   &\frac{d x}{d t}=a x-\alpha x y \\
   &\frac{d y}{d t}=-c y+\gamma x y
   \end{aligned}
   $$
   

3. The **order** of a differential equation is the order of the highest derivative that appears in the equation. 

   For example, below is a 3 order differential equation. 
   $$
   y^{\prime \prime \prime}+2 e^{t} y^{\prime \prime}+y y^{\prime}=t^{4}
   $$

