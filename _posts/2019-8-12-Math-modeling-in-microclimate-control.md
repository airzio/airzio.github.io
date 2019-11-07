---
layout: post
title: Math modeling in microclimate control
comments: true
---
The internal power of the human body can be determined depending on the ambient temperature 

$$P_T=\sum_{i=0}^na_it_B^i$$

In VA Golikov's work [1], this dependence is represented by a second-order equation and the coefficients are determined in the air temperature range from -40 ° C to 55 ° C with a maximum relative error of 14%:

$$P_T=0.04t_B^2-2.37t_B+120$$

The internal capacity of the body can also be determined depending on the heart rate:

$$P_T=aw_c^2+bw_c+c$$

According to VA Golikov's calculations, the coefficients of the equation depend on the body weight. Then the equation takes the form:

$$P_T=(12w_c^2-27.8w_c+18.7)m_T$$

The maximum relative error of approximation was 30% and the average error was 12% for a sample of men aged 20 to 28 years.

The dependence of the heart rate on the ambient temperature for a split non-adapted person air temperature range from -40 ° C to 55 ° C has the form:

$$w_c=2.5 \times 10^{-4} t_B^2+1.33 \times 10^{-3}t_B+0.983$$

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

$$t_sh$$ - temperature of shpere thermometer;

$$t_p=\sqrt[4]{(t_{sh}+273)^4+2.5\sqrt{v_n}(t_{sh}-t_n)\times10^8-273}$$

$$x={ {PT_C-b_0}\over{b_1+0.15(PT_C-t_m)} }$$

$$b_0=\begin{cases}12.2v_n^{0.28} &\text 0.15 \leq v_n \leq 3.5 m/s \\12.75+3.34 ln v_n &\text 3.5 \leq v_n\leq10 m/s\end{cases}$$

$$b_1=4.52-0.34ln v_n$$

$$PT=0.6PT_c+[3.1-0.09(PT_C-t_m)]x-2.4$$ - for dressed people

$$b_0=\begin{cases}12.8+7.6ln v_n &\text 0.15 \leq v_n \leq 3.5 m/s \\17.7+3.9 ln v_n &\text 3.5 \leq v_n\leq10 m/s\end{cases}$$

$$b_1=4.23v_n-0.31$$

From these formulas it is possible to obtain formulas for calculating air parameters at a given value of the resultant temperature and to use them for calculating the task in the comfort controllers.
A mathematical model of the microclimate of a ship's premises with respect to four variables is presented in another paper by VA Golikov:

$$\begin{cases}
{dt_n \over d\tau}={ {Q_{np}+Q_{ex}+Q_{h}+Q_{f}-Q_{yx} } \over {c_p\rho_bV_n} }\\
{dd_n \over d\tau}={ {G_{np}+G_{ex}+G_{h}-G_{yx} } \over {\rho_bV_n} }\\
{dV_n \over d\tau}=\Big({ { {V_{np}+{V_{np}S_{np} \over S_n} \over k_f}-V_{n} } }\Big)k_f^{-2}\\
{dt_f \over d\tau}={F_f\big[{\alpha_bt_n+(K_f+\alpha_n)t_C-(\alpha_b+K_f+\alpha_n)t_f}\big] \over {c_fm_f10^{-3} } }\\
\end{cases}$$

Where $$\rho_b$$- air density kg / m³; $$V_n$$ - the volume of air in the room; $$Q_{np}$$ - heat flow of supply air, kW; $$Q_{ex}$$ - internal heat dissipation; $$Q_h$$ - heat flow that emits a person, kW; $$Q_f$$ - heat flow through the enclosure surfaces; $$Q_{yx}$$ - heat flow from the room; {{d_n}} - humidity in the room; $$G_{np}$$ - moisture introduced by the supply air, relative; $$G_{ex}$$ - humidity in the room air; $$G_h$$ - moisture released by man; $$G_{xy}$$ - moisture exiting the room; $$k_f$$ - inlet entrainment factor, relative; $$S_n$$ - area of ​​the room, $$m^2$$; $$V_{np}$$ - volume of supply air, $$m^3$$; $$S_{np}$$ - inlet area, $$m^2$$; $$F_f$$ - the area of ​​the enclosure surfaces, $$m^2$$; $$t_f$$ - temperature of enclosure surfaces; $$t_C$$ - ambient air temperature; $$\alpha_b$$- coefficient of heat transfer of the enclosing surfaces to the air, W$$m_{-2}$$ °$$С_{-1}$$; $$K_f$$ - heat transfer coefficient of enclosing surfaces, W$$m_{-2}$$ °$$С_{-1}$$; $$\alpha_n$$ - coefficient of heat transfer of the room, W$$m_{-2}$$ °$$С_{-1}$$; $$c_f$$ - heat capacity of the enclosure surfaces, J$$kg_{-1}°C_{-1}$$; $$m_f$$ - the weight of the enclosure surfaces, kg.
This model can be written using transfer functions, which simplifies the simulation of the processes of stabilization of the integral comfort indices PT and PMV, as shown by KV. Khodarina [3].

In the work of A. Ryzhov, H. Ouerdane, E. Gryazina [4] and others for the construction of a microclimate control system using predictive models, a simplified model of the microclimate of the room was applied which does not take into account the change of humidity of air but uses the generation of carbon dioxide by people as a minimum boundary condition flow of supply air

$$\begin{cases}
mC_p{dT \over dt}=U(T-T_{out})+U^*(T^*-T)+W_{oc}N_{oc}\\
m^*C^*{dT^* \over dt}=-U^*(T^*-T)\\
\end{cases}$$
