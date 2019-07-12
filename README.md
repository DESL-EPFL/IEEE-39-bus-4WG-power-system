# IEEE-39-bus-4WG-power-system
A full-replica MATLAB/Simulink dynamic model of the adapted IEEE 39-bus power system, including dynamic models of 10 synchrnonous generations, 4 type-3 wind farms and 19 dynamic loads. 
## New features
* Four type-3 wind farms are added to bus-2, 8, 11, and 21.
* The EPRI LOADSYN model has been adopted as dynamic load model
* M-class cs-TFM PMUs are installed on each load bus for local under frequency load shedding (UFLS)

## Files
### Simulation Model 
The main MATLAB/Simulink model.
### Initialization Files
#### Transmission line parameters
The IEEE 39-bus does not specify any line lengths; therefore, we choose them to obtain a propagation speed just below the speed of light. 
#### Loads profiles
The realistic load profiles are active and reactive components inferred by time series data, adapted from a monitoring system based on Phasor Measurement Units (PMUs) installed in the 125-kV grid of the city of Lausanne, Switzerland. The resolution of the time series is 20 milliseconds and the profiles are voltage and frequency independent. 
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

