#Methods
##System Characterisation
Resistor phantom measurements were carried out in order to assess the noise and drift characteristics of the system. The 32 channel Cardiff phantom \cite{griffiths1995cole} was used, configured to a purely resistive load.  Data was collected using the BioSemi EEG system, in a configuration similar to that used during recordings on the human scalp: with current injected at 2 kHz and 100 $\mu$ A, for 100 ms per measurement, over the course of four hours. The noise, defined as the standard deviation, was considered across three time intervals: 100 repeats (approximately five minutes) representing a typical short term measurement, and one and four hours. These longer recordings replicate the use of the system both in triggered mode, as well as long term monitoring applications \cite{fu2014use} \cite{adler2012whither}.

## Frequency response

The frequency response was determined using two EEG systems, through measurements on a 32 channel resistive phantom with a current of 100 $\mu$ A. A single measurement was averaged across 32 periods for frequencies below 200 Hz and 64 cycles above, with a total of 64 measurement combinations and 10 repeats. Data was collected over a range 20 Hz to 2 kHz, for the BioSemi system and 20 to 20 kHz for the ActiChamp system, and the results normalised to the lowest frequency.  Ideally with a purely resistive test object, no change in voltage should be seen, and the results of these test will be used to calibrate data in all subsequent experiments.

##Experimental Data

Each of the modes of operation previously described have been used in experimental settings. 

### Time difference
\label{methodsTD}
'Standard' time difference EIT data was collected for imaging stroke in a rat model \cite{Dowrick_2016}. Using 100\( \mu \)A at 2kHz and c. 60 injection pairs, a frame of EIT data was recorded every minute, over 30 minutes. A haemorrhage model where blood was injected into the brain over a 10 minute period, was triggered at the 10 minute mark, which was expected to cause a net impedance decrease. EIT images were produced using a 0th order Tikhonov algorithm on a 4 million element mesh of a generic rat skull.

To assess the performance of the system in a clinically realistic scenario, recordings were made in 10 subjects at rest with scalp electrodes. Subjects were fitted with 32 commercial EEG electrodes (EasyCap, Germany, www.easycap.de) configured using the standard EEG 10-20 \cite{Jasper1958} and 10-10 extension \cite{Oostenveld2001} systems. The electrode application procedure was identical to that used in clinical EEG, with each site cleaned with alcohol and abraded before applying conductive paste. Current was injected at 1.2 kHz and 160 $\mu$ A, for 64 cycles or 54 ms, between 31 pairs of electrodes, for a total of 930 measurements for a complete frame. This protocol was repeated 60 times over the course of 20 minutes for each patient. In subsequent analysis, channels below 1 mV standing potential were considered, totalling 540. 

### Triggered

The ScouseTom system was utilised in measurements of evoked activity in the rat somatosensory cortex, following electrical stimulation of the forepaw. The method used closely follows that detailed in \cite{Aristovich_2016} \cite{Vongerichten_2016}, with an increased number of electrodes, from 32 on a single hemisphere to 128 with 64 on each hemisphere. The stimuli delivered were 10 mA pulses 1 ms duration at a rate of 2 Hz, triggered by the ScouseTom controller.

Current was injected at 1.7 kHz with 50 $\mu$ A amplitude, for 30 seconds across a pair of electrodes, with voltages on 127 electrodes recorded in parallel using the ActiChamp ActiveTwo system with 25 kHz sampling rate. The voltages were demodulated with 1 kHz bandwidth, yielding 2 ms time resolution, and coherent averaging was performed on 60 500 ms trials centered around the time of stimulation. This process was repeated for c. 50 pairs of injection electrodes over the course of 25 minutes to produce a complete data set of c. 6000 voltages. EIT images were reconstructed at each 2ms time point in c. 80000 element hexahedral mesh, using the methodology outlined in \cite{Aristovich_2014}.

### Multifrequency 

Multifrequency EIT data was collected as part of clinical trial in collaboration with the Hyper Acute Stroke unit (HASU) at University College London Hospital (UCLH). Stroke patients were fitted with 32 commercial EEG electrodes using the same methodology as described in section \ref{methodsTD}. A total of 31 injection pairs were used, with current injected at 17 frequencies between 5 Hz to 2 kHz, for 32 periods at carrier frequencies below 200 Hz, 64 periods between 200 and 1 kHz, and 128 periods above 1 kHz. The amplitude of injected current varied with frequency as per the guidelines in IEC 60601 \cite{IEC}, with the exception of frequencies below 200 Hz which, as as in previous studies \cite{McEwan_2006}, were reduced by half to ensure the current was not perceptible and to avoid saturation of the EEG amplifier. Given the large number of frequencies and the The protocol was repeated three times, taking a total of 20 minutes to complete. 

A further dataset with 60 repeats using only three frequencies, 200 Hz, 1.2 kHz and 2 kHz, was also recorded on each patient, to better evaluate the frequency dependence of the noise and drift performance of the system. Data were collected in 23 patients, for a total of 31 datasets with 17 frequencies and 29 longer term, 3 frequency recordings. 

### Impedance Spectrum Measurment

Impedance spectrum measurements have been made with the ScouseTom system \cite{Dowrick_2015}, where low frequency (< 3kHz) impedance measurements were made on healthy (n=112 voltage measurments in 4 rats) and ischaemic (n=56 in 2 rats) rat brain. Impedance data was collected using a 100uA injection through two channels of a 30 electrode array, placed directly on the brain surface. The frequency was increased in 5Hz intervals from 1Hz to 100Hz, 10Hz intervals from 100Hz to 1000Hz and 50Hz intervals between 1000Hz and 3000Hz, with a minimum of 50 periods of the waveform recorded at each frequency. The frequency was swept from 1Hz-3000Hz, 3000Hz-1Hz and with random ordering. The use of an EEG recorder allowed parallel voltage recording at all electrodes, which were averaged together at each frequency. The relative change in impedance, rather than the absolute value, was calculated, by comparing the measured voltages at each frequency.
