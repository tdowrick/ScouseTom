# Discussion
A new EIT system has been described which can be utilised in a range of experiments, particularly those involving EIT of the head or nerve. A key advantage of the ScouseTom system is the high level of control it offers over all aspects of the experimental process. This versatility is as a result of the stable performance of the hardware across frequency and load, in particular the current source, which largely removes the need for protocol specific calibration. This calibration has demonstrated substantial benefits with other EIT systems \cite{Hun_Wi_2014} \cite{khan}, but comes at the expense of adaptability.

All of the hardware designs, PCB layouts and associated software have been made available (see Appendix) to allow interested parties to replicate and modify the system. The ScouseTom system is quick to reproduce, as all but two components are commercially available, and the bespoke PCBs are simple compared to those used in other research EIT systems. The major expense is the appropriate EEG system, with the current source and custom PCBs costing around a quarter of the two systems used in this study. Therefore, the additional cost to those already performing electro physiological experiments is minimal, as a large number of common state-of-the-art EEG systems in use are compatible. 

## Summary of results
Noise figures are XXYY
SNR is ZZZZ etc

Four main modes of operation have been utilised, facilitating EIT experiments into imaging of stroke, evoked potentials, epilepsy, activity in peripheral nerves, alongside a range of phantom based investigations.

**comparison to other systems? phantom tests are a bit worse than KHU but about same as UCH. but this system aimed at low freqs and amps, so tests difficult to compare. aim of system is to be verstatile primarily**

## Technical issues
The use of EEG amplifiers for voltage recording limits the maximum frequency to 20kHz, which is sufficient for fast neural EIT, but may not be sufficient for other EIT applications. Additionally, the BioSemi and actiCHamp systems implement hardware antialiasing filters, which causes a reduced gain at higher frequencies \ref{freqresp}. Given that the frequency response of the gain is known, it can easily be accounted for when using multi-frequency data.  


## Recommendations for use