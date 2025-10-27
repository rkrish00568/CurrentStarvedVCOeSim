# Current Starved VCO in eSim
## Abstract
This project focuses on the design and simulation of a Current-Starved Voltage Controlled Oscillator (VCO) using the open-source eSim platform. The circuit employs a CMOS-based ring oscillator topology, where additional current-starving transistors are used to regulate the bias current and control the oscillation frequency through an applied control voltage. By varying this control voltage, the output frequency of the oscillator can be tuned across a wide range. The simulation results demonstrate a clear increase in oscillation frequency with higher control voltage levels, validating the voltage-controlled behavior of the circuit. The designed VCO exhibits stable operation with low power consumption, making it suitable for integration in phase-locked loops (PLLs), frequency synthesizers, and wireless communication systems.

## Reference Circuit Details
The reference design for the Current-Starved Voltage Controlled Oscillator (VCO) is based on a five-stage CMOS ring oscillator topology. Each inverter stage consists of a PMOS–NMOS pair acting as a delay element. To control the current flowing through each inverter stage, additional PMOS and NMOS transistors are connected in series with the supply and ground terminals respectively. These transistors act as current-limiting devices, and the control voltage applied to their gates determines the amount of current available to charge and discharge the load capacitances at each stage.
## Reference Circuit Diagram

![Reference Ckt](images/refckt.png)
## Tools Used:
• esim:  esim design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. esim provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.
![eSim](images/esim.png)
• IHP PDK: The IHP Process Design Kit (PDK) provides a comprehensive set of models, design rules, and libraries for simulating and fabricating CMOS and BiCMOS circuits. It enables accurate analog, digital, and mixed-signal circuit design, supporting advanced nodes like SG13G2 (130 nm). The PDK ensures precise device behavior representation, making it ideal for research and development in high-performance RF, analog, and low-power applications.


## Simulation in esim
### For input V=1volt
![Reference Ckt](images/1v.png)
### For input V=0.7volt
![Reference Ckt](images/0.7v.png)
### For input V=1.5volt
![Reference Ckt](images/1.5v.png)
