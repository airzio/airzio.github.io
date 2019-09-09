---
layout: post
title: Math modeling in microclimate control
comments: true
---

$$P_T=\sum_{i=0}^na_it_B^i$$

$$P_T=0.04t_B^2-2.37t_B+120$$

$$P_T=aw_c^2+bw_c+c$$

$$P_T=(12w_c^2-27.8w_c+18.7)m_T$$

$$w_c=2.5 \times 10^{-4} t_B^2+1.33 \times 10^{-3}t_B+0.983$$

$$PMV=A_0(A_1+A_2d_n+A_3t_p+A_4t_n)$$

$$A_0=0.352e^{-0.036{M_T \over F_{DU} } }+0.032$$

$$A_1=0.39e^{1-1.33\eta}{M_T \over F_{DU} }+5.98-{ {35.7-0.0275(1-\eta){M_T \over F_{DU} } } \over {0.18I} } \times \Big[ 1-{1 \over {A_5} } \Big]$$

$$A_2=411+2.32{M_T \over F_{DU} }$$

$$A_3={3.59f_{OT} \over {A_5} }$$

$$A_4=0.012{M_T \over F_{DU} }+{10.4f_{OT}\sqrt{v_n} \over A_5}$$

$$A_5=1+0.18f_{OT}R_{OD}(3.59+10.4\sqrt{v_n})$$

$$PT={ {PT_C+12.2+[5.94-0.15(PT_C-t_M)]x}\over{2.42-0.032x} }$$

$$PT_C={ {t_p+12.1+(1.7v_n^{0.7}+0.9)t_n}\over{1.7v_n^{0.7}+1.9} }$$

$$t_p=\sqrt[4]{(t_{sh}+273)^4+2.5\sqrt{v_n}(t_{sh}-t_n)\times10^8-273}$$

$$x={ {PT_C-b_0}\over{b_1+0.15(PT_C-t_m)} }$$

$$b_0=\begin{cases}12.2v_n^{0.28} &\text 0.15 \leq v_n \leq 3.5 m/s \\12.75+3.34 ln v_n &\text 3.5 \leq v_n\leq10 m/s\end{cases}$$

$$b_1=4.52-0.34ln v_n$$

$$PT=0.6PT_c+[3.1-0.09(PT_C-t_m)]x-2.4$$

$$b_0=\begin{cases}12.8+7.6ln v_n &\text 0.15 \leq v_n \leq 3.5 m/s \\17.7+3.9 ln v_n &\text 3.5 \leq v_n\leq10 m/s\end{cases}$$

$$b_1=4.23v_n-0.31$$

$$\begin{cases}
{dt_n \over d\tau}={ {Q_{np}+Q_{ex}+Q_{h}+Q_{f}-Q_{yx} } \over {c_p\rho_bV_n} }\\
{dd_n \over d\tau}={ {G_{np}+G_{ex}+G_{h}-G_{yx} } \over {\rho_bV_n} }\\
{dV_n \over d\tau}=\Big({ { {V_{np}+{V_{np}S_{np} \over S_n} \over k_f}-V_{n} } }\Big)k_f^{-2}\\
{dt_f \over d\tau}={F_f\big[{\alpha_bt_n+(K_f+\alpha_n)t_C-(\alpha_b+K_f+\alpha_n)t_f}\big] \over {c_fm_f10^{-3} } }\\
\end{cases}$$

$$\begin{cases}
mC_p{dT \over dt}=U(T-T_{out})+U^*(T^*-T)+W_{oc}N_{oc}\\
m^*C^*{dT^* \over dt}=-U^*(T^*-T)\\
\end{cases}$$