---
layout: post
title: Thermal comfort
comments: true
---
There are several indicies for evaluating the thermal comfort:

- Predicted mean vote (PMV)
- Predicted percentage dissatisfied (PPD)
- Resultant temperature (PT)

## Predicted mean vote

This index was introduced by P.O. Fanger and currently included into **ISO 7730 Standard "Ergonomics of the thermal environment — Analytical determination and interpretation of thermal comfort using calculation of the PMV and PPD indices and local thermal comfort criteria".**
According to standard, PMV may be used for prediction of mean vote of significantly large group of individuals on 7-point sensation scale:

- +3 - Hot
- +2 - Warm
- +1 - Slightly warm
-  0 - Neutral
- −1 - Slightly cool
- −2 - Cool
- −3 - Cold

The calculation of prediction is based on the thermal balance of the body - equality of the heat production in the body and heat loss to the environment. Human thermoregulatory system is capable of adjusting the temperature of the skin and sweat secretion in response to the change of ambient conditions.

$$PMV=\Big[ 0.303⋅e^{-0.036{M} } + 0.028 \Big] \times \\
\Big[ (M - W) - 3.05⋅10^{-3}⋅[5733 - 6.99⋅(M - W) - p_a] - \\
0.42⋅[(M - W) - 58.15] - 1.7⋅10^{-5}⋅M⋅(5867 - p_a) - 0.0014⋅M⋅(34 - t_a) - \\
3.96⋅10^{-8}⋅f_{cl}⋅\Big[ (t_{cl}+273)^4 - (t_r+273)^4 \Big] - f_{cl}⋅h_c⋅(t_{cl}-t_a) \Big]$$

where

$$t_{cl} = 35.7−0.028⋅(M − W) − I_{cl}⋅\Big[3.96⋅10^{-8}⋅f_{cl}⋅\Big[ (t_{cl}+273)^4 - (t_r+273)^4 \Big] + f_{cl}⋅h_c⋅(t_{cl}-t_a) \Big]$$

$$h_c=\begin{cases}2.38⋅|t_{cl} - t_a|^{0.25} &\text for &\text 2.38⋅|t_{cl} - t_a|^{0.25} > 12.1⋅\sqrt{v_{ar}} \\
12.1⋅\sqrt{v_{ar}}  &\text for &\text 2.38⋅|t_{cl} - t_a|^{0.25} < 12.1⋅\sqrt{v_{ar}} \end{cases}$$

$$f_{cl}=\begin{cases}1 + 1.29⋅I_{cl} &\text for &\text I_{cl} \leq 0.078 m^2⋅K/W \\
1.05 + 0.645⋅I_{cl} &\text for &\text I_{cl} > 0.078 m^2⋅K/W \end{cases}$$

M - metabolic rate, ($$W/m^2$$)  
W - effective mechanical power, ($$W/m^2$$)  
$$I_{cl}$$ - clothing insulation, ($$m^2 ⋅ K/W$$)  
$$f_{cl}$$ - clothing surface area factor  
$$t_a$$ - air temperature, (°C)  
$$t_r$$ - mean radiant temperature, (°C)  
$$v_{ar}$$ - relative air velocity, (m/s)  
$$p_a$$ - water vapour partial pressure, (Pa)  
$$h_c$$ - convective heat transfer coefficient, $$[W/(m^2 ⋅ K)]$$  
$$t_{cl}$$ - clothing surface temperature, (°C).  

V.A. Golikov proposed empirical dependencies of the PMV comfort index based on the generalized Fanger equation for air velocity from 0.1 m/s to 0.3 m/s and relative humidity in the range of 30% to 70%

$$PMV=A_0(A_1+A_2d_n+A_3t_p+A_4t_n)$$

where

$$A_0=0.352e^{-0.036{M_T \over F_{DU} } }+0.032$$

$$A_1=0.39e^{1-1.33\eta}{M_T \over F_{DU} }+5.98-{ {35.7-0.0275(1-\eta){M_T \over F_{DU} } } \over {0.18I} } \times \Big[ 1-{1 \over {A_5} } \Big]$$

$$A_2=411+2.32{M_T \over F_{DU} }$$

$$A_3={3.59f_{OT} \over {A_5} }$$

$$A_4=0.012{M_T \over F_{DU} }+{10.4f_{OT}\sqrt{v_n} \over A_5}$$

$$A_5=1+0.18f_{OT}R_{OD}(3.59+10.4\sqrt{v_n})$$

$$d_n$$ - moisture content in the room air  
$$t_p$$ - radiation temperature  
$$t_n$$ - indoor air temperature  
$$f_{OT}$$ - the ratio of the surface of the body of the dressed and undressed person  
$$v_n$$ - Indoor air velocity  
$${ {M_T} \over {F_{DU}} }$$ - specific heat of the person, $$kcal / {{m^2}}$$  
$$\eta$$ - Dressing ratio.

## Predicted percentage dissatisfied
The PPD index is used for prediction of the percentage of thermally dissatisfied people, i.e. people who voted **hot**, **warm**, **cool** or **cold** on the thermal sensation scale mentioned above.

$$PPD=100−95⋅e^{−0.03353⋅PMV^4 −0.2179⋅PMV^2}$$

## Resultant temperature

The Resultant temperature is another measure of comfort. The following equations were also obtained by V.A. Golikov

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

