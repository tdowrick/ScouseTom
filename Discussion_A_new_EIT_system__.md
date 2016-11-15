# Discussion
A new EIT system has been described which can be utilised in a range of experiments, particularly those involving EIT of the head or nerve. A key advantage of the ScouseTom system is the high level of control it offers over all aspects of the experimental process. This versatility is as a result of the stable performance of the hardware across frequency and load, in particular the current source, which largely removes the need for protocol specific calibration. This calibration has demonstrated substantial benefits with other EIT systems \cite{Hun_Wi_2014} \cite{khan}, but comes at the expense of adaptability.

## Summary of results
The system meets with all the criteria described as a reconfigurable system adaptable to a variety of fast neural and brain EIT applications, whilst allowing for extensive control over the measurement setup and data processing. The utilisation of system in four main modes of operation has been outlined, facilitating EIT experiments into time imaging of stroke, multi-frequency stroke type classification, stimulation-triggered evoked potentials. 

Experiments in a resistor phantom with realistic loads demonstrated an SNR of 77.5 dB $\pm$ 1.3 dB when averaged across 100 repeats of a 540 measurement protocol. There were no significant changes in SNR across a four hour recording, or across the frequency range of both EEG systems. The system was able to detect voltage changes of the order of 10s of $\mu$V in both stand EIT time difference and stimulation triggered experiments. Physiological variations and noise, as well as differing hardware setups and data analysis techniques make direct comparison to other EIT systems difficult. However, the results from previous EP studies \cite{Oh2011} in the rat cortex have demonstrated a similar noise level to those recorded with the system described here, suggesting physiological noise is dominant. This is also true for the scalp recordings, where the system noise was masked by physiological noise as well as motion artefacts, although not to the same extent as had been found in previous studies \cite{Fabrizi_2006}. The stability of the system across frequency enabled recording of multi-frequency EIT datasets in stroke patients, as well as impedance spectroscopy type measurements to characterise stroke tissues. Whilst the imaging in these applications is still the subject of research \cite{malone2015} \cite{jang2015detection}, the datasets collected with this system constitute the most comprehensive recorded, and form a basis for future research. 


expanded comparison to other systems. we expect lower SNR based on testing paradigm

cardiff phantom appears noisier
These arise predominantly from temperature changes within the current source, and variations in power supply voltage.

and noise drifts increase from resistor phantom to human - physilogical noise dominates


 The degradation of the SNR using scalp electrodes is in agreement with previous studies \cite{fabrizi2007analysis} which demonstrated system noise accounts for approximately 5 \%, with physiological noise dominating. As with the long term resistor phantom recordings, the drifts across the recordings reduced the equivalent SNR. Additionally, artefacts resulting from subject or electrode movement were present some recordings, further reducing the effective SNR in these cases.  



RE as good as KHU and others

noise in trig same as others - system not limit



Despite the 4-fold increase in bandwidth and consequent noise increase, the performance of the ScouseTom system is comparable to that of previous systems \cite{Oh2011} with 0.37 $\mu$V $\pm$ 0.048 $\mu$V noise across all channels.
 thus meeting the criteria outlined in section \ref{motivation}.

Images obtained previously with a 32 channel system by \citet{Aristovich_2016} with mechanical stimulation of the rat whisker which were found to be in good agreement with established literature, and cross validated with other imaging techniques both in initial onset \cite{armstrong1991thalamo}, and spread of activity \cite{petersen2007functional}. Whilst cross validation was not performed in this study, the literature is equally well established regarding forepaw stimulation, to which these images are in good agreement \cite{peeters2001comparing} \cite{masamoto2007relationship} \cite{lowe2007small}.



The decrease in average SNR compared to the recordings in subjects in section \ref{scalp} is largely a result of a greater prevalence of motion artefacts from patient movement. 


These results were consistent with previous studies in the area \cite{Ranck_1963}, \cite{Logothetis_2007}.

## Technical issues
The use of EEG amplifiers for voltage recording limits the maximum frequency to 20kHz, which is sufficient for fast neural EIT, but may not be sufficient for other EIT applications. Additionally, the BioSemi and actiCHamp systems implement hardware antialiasing filters, which causes a reduced gain at higher frequencies \ref{freqresp}. Given that the frequency response of the gain is known, it can easily be accounted for when using multi-frequency data.

Currently, the majority of the data processing is not performed in "real time", as a complete dataset must be saved to disk. However, as most EEG systems allow for streaming of data via TCP/IP, much of this analysis could be converted to process a single measurement at a time, thus enabling much of the capabilities of other commercial EIT systems.


## Reproducibility and recommendations for use
All of the hardware designs, PCB layouts and associated software have been made available (see Appendix) to allow interested parties to replicate and modify the system. The ScouseTom system is quick to reproduce, as all but two components are commercially available, and the bespoke PCBs are simple compared to those used in other research EIT systems. Within the UCL group, assembly and testing of a new system once all the parts have been acquired can be performed with a week. The major expense is the appropriate EEG system, with the current source and custom PCBs costing around a quarter of the two systems used in this study. Therefore, the additional cost to those already performing electro physiological experiments is minimal, as the system is compatible with  a large number of common state-of-the-art EEG systems. Thus this system greatly reduces the cost and complexity for those interested in including impedance measurements into their experiments.