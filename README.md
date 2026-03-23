# Hydrology-assignment-3
## Part A: Section 1
### Q1
we know $h(x)=c_1*x+c_2$, we find $c_1$ and $c_2$ :

when $x = 0$, $h(x)=c_2$

with the initial condition, we find $c_2=5.8$

when $x=1500$, $h(x)=1500c_1 + 5.8 = 5.4$

$c_1 = \frac{5.4-5.8}{1500} = -0.000267$

Then $h(x)=-0.000267x+5.8$

Since the equation for h(x) is linear, we can expect a linear head profile between the rivers.

### Q3
hydraulic gradient = $c_1$ = $-0.000267$ m

specific discharge, using Darcy's law:

we know that 
$q_x=-K\frac{dh}{dx}$

the specific discharge is : $q_x=1.33*10^{-7}$ 

then we know that $vx=\frac{qx}{n}$, giving us a groudwater velocity $vx=4.04*10^{-7}m.s^{-1}$



## Part A: Section 2
### 1

Because the system is at steady state and there is no source/sink, the specific discharge (Darcy velocity) 𝑞𝑥 must be the same in both zones (conservation of mass). Using Darcy’s law for each zone: 

$q_x=-K1*\frac{hL1-h0}{L1}=-K2*\frac{hL-hL1 }{L2}$

where hL1 is the (unknown) head at the interface 𝑥 = 𝐿1. Equating the two expressions (and dropping the negative signs) gives: 

$K1*\frac{hL1-h0}{L1}=K2*\frac{hL-hL1 }{L2}$

Rearrange the above equation and solve for ℎ𝐿1 using the provided information. 

### 2
###### Zone 1 :
When x=0, $h0=C_2=4m$

Then at $x=L1=500$, $h(L1)=hL1=C_1*500+4$.

-> $C_1=-0.0038$

Which gives for zone 1 : $h(x)=-0.0038x+4$

##### Zone 2: 
When $x=L1$ $h(L1)=hL1 = C1*500+C2 = 2.09$

When $x=L$
$h(L)=hL=C1*(1000)+C2 = 2$

Which mean that : $1000*C1-500*C1=2-2.09$ , $C1=-0.00018$

and $C2=2.09-1000*C1 = 2.18$


### 4
## a)
When $K_1$ is much larger than $K_2$ (e.g., $1000$ vs $10$ m/d), the head profile shifts from a uniform slope to a "stair-step" shape:In Zone 1 (High $K$): Because the material is highly permeable, there is very little resistance to flow. According to Darcy’s Law ($q = -K \frac{dh}{dx}$), a high $K$ requires a very small gradient ($\frac{dh}{dx}$) to move the water. Therefore, the head profile is nearly horizontal (flat), and the interface head ($h_{L1}$) remains very close to $h_0$ ($4.0$ m).In Zone 2 (Low $K$): This zone acts as a flow bottleneck. To move the same volume of water through this resistive material, a much larger "push" is needed. This results in a very steep hydraulic gradient (a sharp drop in the graph).Reference: This follows the linear general solution $h(x) = c_1x + c_2$ mentioned in Assignment 3, Q2, where the slope $c_1$ is inversely proportional to $K$.

## b) 
The specific discharge must be identical ($q_1 = q_2$) due to the Principle of Continuity (Conservation of Mass) for steady-state flow, as shown in your "Groundwater 2" slides (Page 61).Steady-State Requirement: In a steady-state system, the change in storage over time is zero ($\frac{dh}{dt} = 0$). This means the volume of water entering Zone 1 must exactly equal the volume of water leaving Zone 2.Mass Balance: If $q_1$ were greater than $q_2$, water would "pile up" at the interface, causing the head to rise. If $q_1$ were less than $q_2$, a vacuum would form. Since the head is constant in time, the flux must be constant across the entire 1-D path. The equation used:$$K_1 \frac{h_0 - h_{L1}}{L_1} = K_2 \frac{h_{L1} - h_L}{L_2}$$

## Part B
### Q1
### Q2
### Q3
Drawdown Equations: $u=\frac{r^2S}{4Tt}$

$s=\frac{Q}{4πT}\*W(u)$

Solving:
$u=\frac{1000^2\*4E-4}{4\*200\*(365*3)}$

$u=4.57E-4$

Using a look-up table:
$W(u)\approx7.11$

$s=\frac{20}{4π\*200}*7.11$

Drawdown: $s=0.056$ m<sup>3</sup>/day

### Q4
Using the same equations as Q3:

$u=\frac{750^2\*4E-4}{4\*200\*365}$

$u=7.70E-4$

Using a look-up table:
$W(u)\approx6.59$

$s=\frac{15}{4π\*200}*6.59$

$s=0.039$

The total drawdown can then be calculated by superposition:

$s_t = s_1 + s_2$

$s_t = 0.056 + 0.039$

$s_t = 0.095$ m<sup>3</sup>/day
