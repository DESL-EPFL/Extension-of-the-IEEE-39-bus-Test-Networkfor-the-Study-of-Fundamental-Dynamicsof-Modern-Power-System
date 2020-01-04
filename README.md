# Extension of the IEEE 39-bus Test Network for the Study of Fundamental Dynamics of Modern Power System
We provide the full-replica dynamic models of three versions of the IEEE 39-bus power systems, to be used as a benchmark for studying the fundamental dynamics of modern power systems in the presence of inverter-connected devices. 

The up-to-date 4 models correspond to three configurations of the IEEE 39-bus power system with different amount of inertia:

* The original 10-synchronous machine system, noted as Config. I \[[topology](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/modifiedgrid10SG.pdf)\]
* A low-inertia system, 4 synchronous machines are replaced by 4 type-4 wind power plants, noted as Config. II \[[topology](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/modified6SGs4WPs.pdf)\]
* Config. II implemented a Battery Energy Storage Systems (BESS) that integrated into the power grid through a Voltage Source Converter (VSC), noted as Config. II_BESS_VSC \[[topology](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/modifiedgrid4wf6SG1bess.pdf)\]
* A very low-inertia system, 6 synchronous machines are replaced by 6 type-4 wind power plants, noted as Config. III \[[topology](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/modified4SGs6WPs.pdf)\]

Along with the provided dynamic models, we also upload a report where the dynamic models and the corresponding simulation results are presented in details. 

## Files
* [Report](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/Report.pdf) 
* [Dynamic model for Config. I](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/IEEE_39bus_ConfigI.zip)
* [Dynamic model for Config. II](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/IEEE_39bus_ConfigII.zip)
* [Dynamic model for Config. II_BESS_VSC](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/IEEE_39bus_ConfigII_BESS_VSC.zip)
* [Dymamic model for Config. III](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/IEEE_39bus_ConfigIII.zip)
* [Dynamic load model library](https://github.com/DESL-EPFL/Extension-of-the-IEEE-39-bus-Test-Networkfor-the-Study-of-Fundamental-Dynamicsof-Modern-Power-System/blob/master/IEEE_39Bus_dynload_lib.mdl.zip)

## Simulation notes
* It is recommend to use Phasor Measurement Unit ( PMU) to measure phasor, frequency and ROCOF. In another project [CS-TFM PMU model](https://github.com/DESL-EPFL/CS-TFM-PMU-Model.git), we provide the PMU models that relie on Compressive Sensing Taylor-Fourier Model (CS-TFM) approach
* It is worth to note that, due to the limitation of Syncrhonous Machine block in discrete system in MATLAB/Simulink, it is necessary to use a small parasitic resistive load, connected at the machine terminals, to avoid numerical oscillations. Details regarding how to use parasitic resistive load,see in [Mathwork](https://mathworks.com/help/physmod/sps/powersys/ref/synchronousmachine.html).
 

## Real-time simulator 
We use the Opal-RT real-time digital simulator OP5600, coupled with the eMEGAsim PowerGrid running on the RT-LAB real-time simulation platform. For installation, user guide and more information on the real-time simulator go [here](https://www.opal-rt.com/).

## Software 
The following software is required to run the model:
* MATLAB Version 8.5.1 (R2015aSP1)   
* Simulink Version 8.5.1 (R2015aSP1)   
* ARTEMIS Blockset Version 7.2.2.1206 (R2015a)   
* RT-LAB Version v11.2.2.108 (R2015a.x), available [here](https://www.opal-rt.com/)

## References 
For a more detailed description of this full-replica IEEE 39-bus system model, refer to the following references:
* Yihui Zuo, Fabrizio Sossan, Mokhtar Bozorg, Mario Paolone, “Dispatch and Primary Frequency Control with Electrochemical Storage: a System-wise Verification,” IEEE PES Innovative Smart Grid Technologies Conference Europe (ISGT-Europe), 2018. Available [here](https://ieeexplore.ieee.org/document/8571832).
* Yihui Zuo, Guglielmo Frigo, Asja Derviškadić and Mario Paolone, "Impact of Synchrophasor Estimation Algorithms in ROCOF-based Under-Frequency Load-Shedding," in IEEE Transactions on Power Systems. Available [here](https://ieeexplore.ieee.org/document/8807346).
* Asja Derviškadić, Yihui Zuo, Guglielmo Frigo, Mario Paolone, “Under Frequency Load Shedding based on PMU Estimates of Frequency and ROCOF,” IEEE PES Innovative Smart Grid Technologies Conference Europe (ISGT-Europe), 2018. Available [here](https://ieeexplore.ieee.org/document/8571481).
* Guglielmo Frigo, Asja Derviškadić, Yihui Zuo and Mario Paolone, "PMU-Based ROCOF Measurements: Uncertainty Limits and Metrological Significance in Power System Applications," in IEEE Transactions on Instrumentation and Measurement. Available [here](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8675542&isnumber=4407674).

