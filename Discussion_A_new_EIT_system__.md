# Discussion
A new EIT system has been described which can be utilised in a range of experiments, particularly those involving EIT of the head or nerve. A key advantage of the ScouseTom system is the high level of control it offers over all aspects of the experimental process. This versatility is as a result of the stable performance of the hardware across frequency and load, in particular the current source, which largely removes the need for protocol specific calibration. This calibration has demonstrated substantial benefits with other EIT systems \cite{Hun_Wi_2014} \cite{khan}, but comes at the expense of adaptability.

## Summary of results

Experiments in a resistor phantom with realistic loads demonstrated an SNR of 77.5 dB $\pm$ 1.3 dB when averaged across 100 repeats of a 540 measurement protocol. There were no significant changes in SNR across a four hour recording, or across the frequency range of both EEG systems.

The utilisation of system in four main modes of operation has been outlined, facilitating EIT experiments into time imaging of stroke, multi-frequency stroke type classification, stimulation-triggered evoked potentials. The system was able to detect voltage changes of the order of 10s of $\mu$V in both stand EIT time difference and stimulation triggered experiments. Physiological variations and noise, as well as differing hardware setups and data analysis techniques make direct comparison to other EIT systems difficult. However, the results from previous EP studies \cite{Oh2011} in the rat cortex have demonstrated a similar noise level to those recorded with the system described here, suggesting physiological noise is dominant. This is also true for the scalp recordings, where the system noise was masked by physiological noise as well as motion artefacts, although not to the same extent as had been found in previous studies \cite{Fabrizi_2006}. The stability of the system across frequency enabled recording of multi-frequency EIT datasets in stroke patients, as well as impedance spectroscopy type measurements to characterise stroke tissues. Whilst the imaging in these applications is still the subject of research \cite{malone2015} \cite{jang2015detection}, the datasets collected with this system constitute the most comprehensive recorded, and form a basis for future research. 

The system 
Further experiments investigating epilepsy, activity in peripheral nerves. 



## Technical issues
The use of EEG amplifiers for voltage recording limits the maximum frequency to 20kHz, which is sufficient for fast neural EIT, but may not be sufficient for other EIT applications. Additionally, the BioSemi and actiCHamp systems implement hardware antialiasing filters, which causes a reduced gain at higher frequencies \ref{freqresp}. Given that the frequency response of the gain is known, it can easily be accounted for when using multi-frequency data.  


## Recommendations for use
All of the hardware designs, PCB layouts and associated software have been made available (see Appendix) to allow interested parties to replicate and modify the system. The ScouseTom system is quick to reproduce, as all but two components are commercially available, and the bespoke PCBs are simple compared to those used in other research EIT systems. The major expense is the appropriate EEG system, with the current source and custom PCBs costing around a quarter of the two systems used in this study. Therefore, the additional cost to those already performing electro physiological experiments is minimal, as the system is compatible with  a large number of common state-of-the-art EEG systems. Thus this system greatly reduces the cost and complexity for those interested in including impedance measurements into their experiments.