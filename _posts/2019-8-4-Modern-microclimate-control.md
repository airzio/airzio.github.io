---
layout: post
title: Modern microclimate control
comments: true
---

Safe and comfort microclimate in living and working premisses is crucially important for human health and mental ability. Optimal performance at work and proper rest at home is not possible without clean air of comfort temperature and humidity.

Modern microclimate control concepts are general for various types of inhabited premisses, included ones of transport vehicles, but safe and comfort levels are governed by different standards and regulations depending on the type and purpose of the room or compartment.

There are a number of structural and operational requirements for microclimate and ventilation systems, which are defined in international standards [1-4] and national standards and regulations. The microclimate of the premises should be maintained not only comfortable but first of all safe. Microclimate safety means the compliance of temperature, humidity, mobility and gas composition of air with international standards and norms. The requirements for measuring the gas composition of the air are established by the international standards ISO16000-1 - ISO16000-38, which regulate the methods of measuring the content of various contaminants in the air. A new standard - ISO / FDIS Standard 16000-40 Indoor air quality management system is in the process of being approved.

Let take a look at theoretical principles for the control of the microclimate which developed by various scientific schools.

The peculiarity of the microclimate concept, proposed by V. Golikov [5], is to define a human body as an object of the control. Accordingly, the temperature, humidity and air velocity of the air act as a controlling influences on a person's well-being. From the standpoint of this concept, the characteristics of the microclimate of the premises were investigated and a generalized mathematical model of human adaptation processes was developed.

For the inhabited premisses, the following mathematical models were composed and studied:

- linear distributed microclimate model
- nonlinear distributed microclimate model
- concentrated parameters model
- model of living quarters air pressure dynamics
- indoor air pollution model

For the purpose of the microclimate automated control, V. Golikov [5] proposed a mathematical model in the form of systems of differential equations with three variables: the temperature and humidity of the supply air and the resulting temperature. As a result of the model study, it was determined that classic P, PI and PID controllers are not capable of keeping all three process variables in the required limits. To overcome this limitation, the mathematical model of the microclimate with the concentrated parameters and principle of maximum in the optimal performance problem were applied. The optimal relay regulator was synthesized, in which the control flow is mathematically expressed as a piecewise constant function. The coefficients of the piecewise constant function were determined by the Box's method. The received controller allows to keep the resulting temperature and microclimate parameters within the set limits.

K. Khodarina [6] applied the concept of microclimate proposed by Golikov for the study of the relationship between the integral comfort index PMV and the resulting temperature PT. She proposed empirical formulas for the PMV calculation as a function of PT. The resulting temperature stabilization algorithm was developed using a multivariable control effect on the inhabited premisses atmosphere.

The proposed climate control system includes:

- a calculation block that calculates the set point for PID regulators for each of the controlled parameters applying the Nedler-Mead method
- PID regulators for each of the controlled parameters

Controlled parameters are as follows:

- temperature
- humidity
- air velocity
- temperature of the surfaces in the room

The simulation of integral comfort index PMV dynamic and stabilization revealed that the optimal strategy for influencing the atmosphere of the room is a method of regulating the temperature and velocity of the supply air by the criterion of the minimum quadratic deviation of the resulting temperature.

K. Khodarin and Zherlytsin OV [7] proposed a scheme for microclimate evaluation which based on a neural network.
According to the authors, the microclimate state can be evaluated  predicted by the neural networks by applying the pattern recognition methods. The proposed system should use a database to store sensor data and two neural networks: predictive and diagnostic. Measured values  of microclimate parameter  will be input to the diagnostic network, and the network output will be a generalized indicator of the microclimate status on some scale developed during the network training. The predictive neural network will analyze recorded in the database microclimate parameter time series and provide a predicted microclimate status at the output with the desired bias that will allow the control unit to generate the desired control action value.

Researchers A. Ryzhov, H. Ouerdane, E. Gryazina [8] and others have applied control principles with predictive MPC models to control the microclimate parameters by the criterion of energy minimization. The main advantages of the MPC method used are its ability to take into account foreseeable external factors (weather and occupancy forecasts) and limitations such as air conditioning system power, minimum airflow to control carbon dioxide content, minimum and maximum comfort zone temperature. The effectiveness of using the full forecast model compared to the linearized forecast model and relay controller was analyzed. It is determined that the use of nonlinear forecasting models is the most appropriate to ensure the desired comfort level and minimum energy consumption. The use of the proposed models also allows the preliminary preparation of the microclimate of the premises, taking into account weather forecasts and occupancy of the premises.

Most often inhabited premises in buildings or transportation vehicles have adjacent to some number of neighbor rooms or compartments. The microclimate of each of the premises and all of them as a whole should be considered as a comprehensive task of optimizing the air parameters in several controlled areas. [Xuan Zhang, Wenbo Shi, and others [9] proposed a decentralized real-time microclimate control system. The purpose of the system control is to balance the energy costs and the comfort of the room. The theoretical basis of the system is a thermodynamic model of resistance-capacity (RC model) for a number of adjacent premises, which allows to apply the task of static resources distribution for the purpose of energy saving by controlling the distribution of air. Gradient algorithms were used to solve the problem of static resource allocation. A feature of the proposed technique is the use of dynamic feedback controllers that implement decentralized and distributed algorithms for the adaptation of air flow into each of the monitored premises. Unlike controls based on predictive models, such controllers, due to the thermodynamic model used, do not require explicit consideration of disturbances, such as changes in ambient air parameters, room occupancy, and internal heat generation.

One of the most promising approaches to climate control is to use fuzzy logic control systems. In the study of researchers Md. Fakhruddin H.N. , Syed Akbar Ali and others [10] it had been proposed a system with fuzzy logic for climate control. The controller will receive user-defined temperature, current indoor temperature, dew point temperature, room occupancy (number of people) and time of day (morning, afternoon, night) as the input. At the output, the controller calculates the compressor and fan load, operating mode (temperature or humidity control) and air flow direction. The controller consists of normalize input parameters database, a database of fuzzy rules, a kernel of fuzzy output, and a decoder that converts the fuzzy controller outputs into the actuator command signals. The output values ​​of the controller are calculated using 18 matrixes of heuristic rules.

Reviewed microclimate control methods are not designed to ensure the comfortable and safe microclimate simultaneously. By comfortable microclimate we understand that all it's parameters - temperature, humidity and air velocity - are in comfort limits. By safe microclimate we understand that it does not contain any pollutants with concentrations above safe limits.  It the necessity to improvement the existing microclimate management method by including the control of air quality parameters.

## References

1. ANSI/ASHRAE Standard 62.1-2016, Ventilation for Acceptable Indoor Air Quality.  
2. ISO 7547. Ships and marine technology -- Air-conditioning and ventilation of accommodation spaces -- Design conditions and basis of calculations
3. ISO 8862. Air-conditioning and ventilation of machinery control-rooms on board ships -- Design conditions and basis of calculations
4. ISO 8864. Air-conditioning and ventilation of wheelhouse on board ships -- Design conditions and basis of calculations
5. Голиков В. А. Повышение эффективности и оптимизация режимов работы систем судового микроклимата: дис. на соиск. науч. степ. док-ра техн. наук: спец. 05.08.05 "Судовые энергетические устновки" / В. А. Голиков - 2000.
6. Ходарина К. В. Обеспечение комфортных условий микроклимата обитаемых помещений морских судов:  дис. на соиск. уч. степ. канд. техн. наук: спец. 05.22.20 "Эксплуатация и ремонт средств транспорта" / К. В. Ходарина - 2013
7. Ходаріна К.В., Жерліцина О.В. Автоматизована діагностика суднового мікроклімату з використанням апарату нейронних сітей. // ВІСНИК ПРИАЗОВСЬКОГО ДЕРЖАВНОГО ТЕХНІЧНОГО УНІВЕРСИТЕТУ. - 2011. - Вип. 22. - С 236 - 240
8. Ryzhov, A & Ouerdane, Henni & Gryazina, Elena & Bischi, Aldo & Turitsyn, K. (2018). Model predictive control of indoor microclimate: Existing building stock comfort improvement. Energy Conversion and Management. 179. 10.1016/j.enconman.2018.10.046. 
9. Xuan Zhang, Wenbo Shi, Bin Yan, Ali Malkawi and Na Li. (2017). Decentralized and Distributed Temperature Control via HVAC Systems in Energy Efficient Building
10. Md. Fakhruddin H.N. , Syed Akbar Ali, Mohd.Muzafarб Dr. Syed Azam pasha Quadri. (2016). Fuzzy Logic in HVAC for Human Comfort
