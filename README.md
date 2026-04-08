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
The specific discharge must be identical ($q_1 = q_2$) due to the Principle of Continuity (Conservation of Mass) for steady-state flow, as shown in your "Groundwater 2" slides (Page 61).Steady-State Requirement: In a steady-state system, the change in storage over time is zero ($\frac{dh}{dt} = 0$). This means the volume of water entering Zone 1 must exactly equal the volume of water leaving Zone 2.Mass Balance: If $q_1$ were greater than $q_2$, water would "pile up" at the interface, causing the head to rise. If $q_1$ were less than $q_2$, a vacuum would form. Since the head is constant in time, the flux must be constant across the entire 1-D path. The equation used: $$K_1 \frac{h_0 - h_{L1}}{L_1} = K_2 \frac{h_{L1} - h_L}{L_2}$$

## Part B
### Q1
For steady-state one-dimensional flow in a confined aquifer with no sources or sinks, the governing equation is:

$\frac{d}{dx}\left(T \frac{dh}{dx}\right) = 0$

Assuming constant transmissivity $T$, this simplifies to:

$\frac{d^2 h}{dx^2} = 0$

From here we integrating twice which gives us:

$\frac{dh}{dx} = C_1$

$h(x) = C_1 x + C_2$

Now we can apply the boundary conditions:

We know that at the left river $x = 0$:

$h(0) = 32.0$

And for the right river we have $x = 2400$:

$h(2400) = 25.5$

By substitute the first condition we get:

$h(0) = C_1(0) +C_2 = 32.0$

And:

$C_2 = 32.0$

Now we can use the second condition which gives us:

$h(2400) = C_1(2400) + 32.0 = 25.5$

$2400C_1 = 25.5 - 32.0 = -6.5$

$C_1 = \frac{-6.5}{2400} = -0.00270833$

Therefore, the hydraulic head distribution is:

$h(x) = 32.0 - 0.00270833\,x$

Or as:

$h(x) = 32.0 + \frac{25.5 - 32.0}{2400}\,x$

### Q2
The data we have are:
Pumping rate:

$Q = 54 \ \text{m}^3/\text{hr}$

And the observation well distance from pumping well:

$r = 20 \ \text{m}$

Now we use the Theis solution:

$s = \frac{2.3Q}{4\pi T} \log_{10}\left(\frac{2.25Tt}{r^2 S}\right)$

This is why plotting $s$ versus $\log_{10}(t)$ gives a straight line. Which can be seen below:

Plot:
<img width="830" height="555" alt="image" src="https://github.com/user-attachments/assets/5bce0236-71c5-4c5f-b5eb-f8db6c08cfa0" />

From that straight line we can see that it slope over one log cycle, $\Delta s$, gives $T$. The time-axis intercept $t_0$ gives $S$. With:

$T = \frac{2.3Q}{4\pi \Delta s}$

$S = \frac{2.25Tt_0}{r^2}$

Using $t$ in minutes:

| $t$ (min) | $\log_{10}(t)$ | $s$ (m) |
|----------|----------------|--------|
| 1.67     | 0.223          | 0.6    |
| 5        | 0.699          | 1.2    |
| 10       | 1.000          | 1.5    |
| 16.67    | 1.222          | 1.7    |
| 50       | 1.699          | 2.3    |
| 83.33    | 1.921          | 2.5    |
| 133.33   | 2.125          | 2.8    |
| 200      | 2.301          | 3.0    |

These points are close to a straight line on semilog paper. A fitted straight line is approximately:

$s \approx 1.14 \log_{10}(t) + 0.356$

This means that the drawdown increase over one log cycle is:

$\Delta s \approx 1.14 \ m$

We therefore use:

$T = \frac{2.3Q}{4\pi \Delta s}$

Since time data are in minutes, we convert pumping rate:

$Q = 54 \ \text{m}^3/\text{hr} = 0.9 \ \text{m}^3/\text{min}$

Now we can substitute:

$T = \frac{2.3(0.9)}{4\pi (1.14)}$

$T \approx 0.145 \ \text{m}^2/\text{min}$

With the straight-line equation being:

$s = 1.14 \log_{10}(t) + 0.356$

At the intercept $s = 0$:

$0 = 1.14 \log_{10}(t_0) + 0.356$

$\log_{10}(t_0) = -\frac{0.356}{1.14} \approx -0.312$

$t_0 = 10^{-0.312} \approx 0.487 \ \text{min}$

So:

$t_0 \approx 0.49 \ \text{min}$

We use:

$S = \frac{2.25Tt_0}{r^2}$

Use consistent units:

- $T = 0.145 \ \text{m}^2/\text{min}$

- $t_0 = 0.487 \ \text{min}$

- $r = 20 \ \text{m}$

With this data we can substitute:

$S = \frac{2.25(0.145)(0.487)}{20^2}$

$S \approx 3.96 \times 10^{-4}$

Which gives us:

$S \approx 4.0 \times 10^{-4}$

$T \approx 0.145 \ \text{m}^2/\text{min}$

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


# Part C 
### Q1 
We observe that as the distance from the pumping well increases, the drawdown decrease. 
Similarly, as the vertical position increases, the drawdown increases. For example, the wells C0134-2-1 and C0134-2-2 are at the same distance from the pumping well, but the vertical position of the first one is about -2 m against -1 m for the second. The first one has a bigger drawdown. This phenomenon can mean that the aquifer is stratified.

Most of the time, the drawdown value stabilizes before it decreases after a certain time with various recovery times when the pumping stops.

### Q3 
The Theis solution cannot be used for the pumping well itself since it is considering the distance from the well in the formula. 
Also, as the Theis solution is made for confined aquifers, for wells with 1–3 m below ground, the wells are almost certainly sitting in the unsaturated zone or are unconfined aquifers, which makes the Theis solution unusable.

### Q4
Based on the curve-fitting of the Theis analytical solution to the observed drawdown data at well C0121-2-1, the best estimates for the aquifer properties are:
- Transmissivity (T): 6.28e-04 m²/s (approximately $6.3 \times 10^{-4}$ m²/s)
- Storativity (S): 1.15e-03
These values are highly characteristic of the Copenhagen Limestone aquifer. A transmissivity in the $10^{-4}$ range indicates a moderately productive fractured limestone aquifer. The storativity value of roughly 0.001 confirms that the aquifer is under confined or semi-confined conditions, as unconfined aquifers typically have much higher storativity (specific yield) values (closer to 0.1 to 0.3).
<img width="762" height="583" alt="image" src="https://github.com/user-attachments/assets/51d617be-0fbc-47e9-abd1-c0e1c52cd952" />


### Q5
The Theis solution provides a reasonable baseline fit for the early stages of pumping, however, it assumes a perfectly homogeneous, isotropic, fully confined aquifer with no recharge. Real-world data from the Copenhagen Metro site typically deviates from this ideal curve at later times.
Based on the site's geology and hydrogeological principles, the deviations which means where the black observation dots separate from the red Theis line, can be attributed to the following factors:
- Double-Porosity (Fractured Flow): The Copenhagen Limestone is a dual-porosity medium. When pumping starts, water is rapidly depleted from the high-permeability fractures (creating early steep drawdown). Later, water slowly drains from the low-permeability rock matrix into the fractures. This transition causes the actual drawdown curve to temporarily flatten or form an "inflection point" that a standard Theis curve cannot capture.
- Leaky Aquifer Conditions: The limestone aquifer is overlain by glacial units (such as clay till and sand). As pumping continues and the pressure drops in the limestone, water from these overlying aquitards begins to leak downward into the primary aquifer. This extra source of water causes the observed drawdown to flatten out at late times compared to the continuous drop predicted by the Theis model.
- Boundary Effects: If the drawdown cone extends far enough to intersect a constant-head boundary such as the nearby Copenhagen harbour or a fully penetrating river, the drawdown will stabilise completely. Conversely, if it hits an impermeable barrier such as a geological fault, the drawdown would steepen abruptly.
