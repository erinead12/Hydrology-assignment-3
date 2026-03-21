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

## Part B
### Q1
### Q2
### Q3
Drawdown Equations: $u=\frac{r^2S}{4Tt}$

$s=\frac{Q}{4πT}\*W(u)$
Solving:
$u=\frac{1000^2\*4E-4}{4\*200*365}$
$u=1.37E-3$

Using a look-up table:
$W(u)\approx6.10$

$s=\frac{20}{4π\*200}*6.10$

$s=0.048$ m<sup>3</sup>/day
