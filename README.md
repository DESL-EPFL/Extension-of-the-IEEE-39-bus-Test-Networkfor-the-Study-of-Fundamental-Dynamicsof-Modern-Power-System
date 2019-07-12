# Extension-of-the-IEEE-39-bus-Test-Network-for-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System

In the report, we detaily describe three versions of full-replica dynamic models of the IEEE 39-bus power systems, to be used as a benchmark for studying the fundamental dynamics of modern power systems inthe presence of inverter-connected devices.
The models correspond to three configurations of the IEEE39-bus power system:

* The original 10-synchronous machine system, noted as Config. I
* An inertia-reduced system, including wind power plants, noted as Config. II
* An inertia-reduced system, including wind power plants and Battery Energy Storage Systems(BESS), noted as Config. III

## Files
* [Dynamic model for Configuration I](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/IEEE_39Bus_configI.zip)
* [Dynamic model for Configuration II](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/IEEE_39Bus_configII.zip)
* [Dymamic model for Configuration III](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/IEEE_39Bus_configIII.zip)



## Real-time simulator 
We use the Opal-RT real-time digital simulator OP5600, coupled with the eMEGAsim PowerGrid running on the RT-LAB real-time simulation platform. For installation, user guide and more information of the real-time simulator go [here](https://www.opal-rt.com/).
## Software 
The following software is required to run the model:
* MATLAB Version 8.5.1 (R2015aSP1)   
* Simulink Version 8.5.1 (R2015aSP1)   
* ARTEMIS Blockset Version 7.2.2.1206 (R2015a)   
* RT-LAB Version v11.2.2.108 (R2015a.x), available [here](https://www.opal-rt.com/)

## References 
For a more detailed description of this full-replica IEEE 39-bus system model, refer to the following references:
* Yihui Zuo, Fabrizio Sossan, Mokhtar Bozorg, Mario Paolone, “Dispatch and Primary Frequency Control with Electrochemical Storage: a System-wise Verification,” IEEE PES Innovative Smart Grid Technologies Conference Europe (ISGT-Europe), 2018. Available [here](https://ieeexplore.ieee.org/document/8571832).
* Asja Derviškadić, Yihui Zuo, Guglielmo Frigo, Mario Paolone, “Under Frequency Load Shedding based on PMU Estimates of Frequency and ROCOF,”IEEE PES Innovative Smart Grid Technologies Conference Europe (ISGT-Europe), 2018. Available [here](https://ieeexplore.ieee.org/document/8571481).
* G. Frigo, A. Derviškadić, Y. Zuo and M. Paolone, "PMU-Based ROCOF Measurements: Uncertainty Limits and Metrological Significance in Power System Applications," in IEEE Transactions on Instrumentation and Measurement. Available [here](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8675542&isnumber=4407674).

