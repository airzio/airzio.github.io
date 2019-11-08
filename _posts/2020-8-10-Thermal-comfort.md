---
layout: post
title: Thermal comfort
comments: true
---
There are several indicies for evaluating the thermal comfort:

- Predicted mean vote (PMV)
- Predicted percentage dissatisfied (PPD)
- Resultant temperature (PT)

 ##Predicted mean vote

This index was introduced by P.O. Fanger and currently included into ISO 7730 Standard "Ergonomics of the thermal environment — Analytical determination and interpretation of thermal comfort using calculation of the PMV and PPD indices and local thermal comfort criteria".
According to standard, PMV may be used for prediction of mean vote of significantly large group of individuals on 7-point sensation scale:

- +3 - Hot
- +2 - Warm
- +1 - Slightly warm
-  0 - Neutral
- −1 - Slightly cool
- −2 - Cool
- −3 - Cold

The prediction calculation, is based on the thermal balance of the body - equality of the heat production in the body and heat loss to the environment. Human thermoregulatory system is capable of adjusting the temperature of the skin and sweat secretion in response to the change of ambient conditions.

$$PMV=\Big[ 0.303 e^{-0.036{M} } + 0.028 \Big] \times \\
\Big[ (M - W) - 3.05 \times 10^{-3} \times [5733 - 6.99⋅(M - W) - p_a] - \\
0.42⋅[(M - W) - 58.12] - 1.7⋅10^{-5}⋅M⋅(5867 - p_a) - 0.0014⋅M⋅(34 - t_a) - \\
3.96⋅10^{-8}⋅f_{cl}⋅\Big[ (t_{cl}+273)^4 - (t_r+273)^4 \Big] - f_{cl}⋅h_c⋅(t_{cl}-t_a) \Big]$$

where

$$t_{cl} = 35.7−0.028⋅(M − W) − I⋅\Big[3.96⋅10^{-8}⋅f_{cl}⋅\Big[ (t_{cl}+273)^4 - (t_r+273)^4 \Big] + f_{cl}⋅h_c⋅(t_{cl}-t_a) \Big]$$

$$h_c=\begin{cases}2.38⋅(t_{cl} - t_a)^0.25 &\text for 2.38⋅(t_{cl} - t_a)^0.25 > 12.1⋅sqrt{v_{ar}} \\ 12.1⋅sqrt{v_{ar}}  \text for 2.38⋅(t_{cl} - t_a)^0.25 < 12.1⋅sqrt{v_{ar}} \end{cases} $$

$$f_{cl}=\begin{cases}1 + 1.29⋅I_{cl} &\text for I_{cl} \leq 0.078 m^2⋅K/W \\ 1.05 + 0.645⋅I_{cl} &\text for I_{cl} > 0.078 m^2⋅K/W \end{cases}$$

M - the metabolic rate, ($$W/m^2$$)
W - the effective mechanical power, ($$W/m^2$$)
$$I_{cl}$$ - the clothing insulation, ($$m^2 ⋅ K/W$$)
$$f_{cl}$$ - the clothing surface area factor
$$t_a$$ - the air temperature, (°C)
$$t_r$$ - the mean radiant temperature, (°C)
$$v_{ar}$$ - the relative air velocity, (m/s)
p_a - the water vapour partial pressure, (Pa)
h_c - the convective heat transfer coefficient, $$[W/(m^2 ⋅ K)]$$
t_{cl} - the clothing surface temperature, (°C).

Empirical dependencies of the PMV comfort index are obtained from the generalized Fanger equation for air velocity from 0.1 m / s to 0.3 m / s and relative humidity in the range of 30% to 70%

$$PMV=A_0(A_1+A_2d_n+A_3t_p+A_4t_n)$$

where

$$A_0=0.352e^{-0.036{M_T \over F_{DU} } }+0.032$$

$$A_1=0.39e^{1-1.33\eta}{M_T \over F_{DU} }+5.98-{ {35.7-0.0275(1-\eta){M_T \over F_{DU} } } \over {0.18I} } \times \Big[ 1-{1 \over {A_5} } \Big]$$

$$A_2=411+2.32{M_T \over F_{DU} }$$

$$A_3={3.59f_{OT} \over {A_5} }$$

$$A_4=0.012{M_T \over F_{DU} }+{10.4f_{OT}\sqrt{v_n} \over A_5}$$

$$A_5=1+0.18f_{OT}R_{OD}(3.59+10.4\sqrt{v_n})$$

$$d_n$$ - moisture content in the room air; $$t_p$$ - radiation temperature; $$t_n$$ - indoor air temperature; $$f_OT$$ - the ratio of the surface of the body of the dressed and undressed person; $$v_n$$ - Indoor air velocity; $${ {M_T} \over {F_DU} }$$ - specific heat of the person, kcal / {{m^2}}; {{\nu}}- Dressing ratio.

For another measure of comfort - the resultant temperature - empirical dependencies were also obtained:

$$PT={ {PT_C+12.2+[5.94-0.15(PT_C-t_M)]x}\over{2.42-0.032x} }$$ - for undressed people

Where $$t_M$$is the temperature of the wet thermometer;

$$PT_C={ {t_p+12.1+(1.7v_n^{0.7}+0.9)t_n}\over{1.7v_n^{0.7}+1.9} }$$ - dry resultive temperature;

$$t_sh$$ - themperature of sphere thermometer;

$$t_p=\sqrt[4]{(t_{sh}+273)^4+2.5\sqrt{v_n}(t_{sh}-t_n)\times10^8-273}$$

$$x={ {PT_C-b_0}\over{b_1+0.15(PT_C-t_m)} }$$

$$b_0=\begin{cases}12.2v_n^{0.28} &\text 0.15 \leq v_n \leq 3.5 m/s \\12.75+3.34 ln v_n &\text 3.5 \leq v_n\leq10 m/s\end{cases}$$

$$b_1=4.52-0.34ln v_n$$

$$PT=0.6PT_c+[3.1-0.09(PT_C-t_m)]x-2.4$$ - for dressed people

$$b_0=\begin{cases}12.8+7.6ln v_n &\text 0.15 \leq v_n \leq 3.5 m/s \\17.7+3.9 ln v_n &\text 3.5 \leq v_n\leq10 m/s\end{cases}$$

$$b_1=4.23v_n-0.31$$

