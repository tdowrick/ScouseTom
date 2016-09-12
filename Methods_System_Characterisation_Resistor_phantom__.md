#Methods
##System Characterisation
Resistor phantom measurements were carried out in order to assess the noise and drift characteristics of the system. The 32 channel Cardiff phantom \cite{griffiths1995cole} was used, configured to a purely resistive load.  Data was collected using the BioSemi EEG system, in a configuration similar to that used during recordings on the human scalp: with current injected at 2 kHz and 100 $\mu$ A, for 100 ms per measurement, over the course of four hours. The noise, defined as the standard deviation, was considered across three time intervals: 100 repeats (approximately five minutes) representing a typical short term measurement, and one and four hours. These longer recordings replicate the use of the system both in Triggered mode, as well as long term monitoring applications \cite{fu2014use} \cite{adler2012whither}.


## Frequency response

The frequency response was determined using two EEG systems, through measurements on a 32 channel resistive phantom with a current of 100 $\mu$ A. A single measurement was averaged across 32 periods for frequencies below 200 Hz and 64 cycles above, with a total of 64 measurement combinations and 10 repeats. Data was collected over a range 20 Hz to 2 kHz, for the BioSemi system and 20 to 20 kHz for the ActiChamp system, and the results normalised to the lowest frequency.  Ideally with a purely resistive test object, no change in voltage should be seen, and the results of these test will be used to calibrate data in all subsequent experiments.

##Modes/Experimental Data

Each of the modes of operation previously described have been used in experimental settings. 

### Time difference
'Standard' time difference EIT data was collected for imaging stroke in a rat model \cite{Dowrick_2016}. Using 100\( \mu \)A at 2kHz and c. 60 injection pairs, a frame of EIT data was recorded every minute, over 30 minutes. A haemorrhage model where blood was injected into the brain over a 10 minute period, was triggered at the 10 minute mark, which was expected to cause a net impedance decrease.

### Triggered

The ScouseTom system was utilised in measurements of evoked activity in the rat somatosensory cortex, following electrical stimulation of the forepaw. The method used closely follows that detailed in \cite{Aristovich_2016} \cite{Vongerichten_2016}, with an increased number of electrodes, from 32 on a single hemisphere to 128 with 64 on each hemisphere. The stimuli delivered were 10 mA pulses 1 ms duration at a rate of 2 Hz, triggered by the ScouseTom controller.

Current was injected at 1.7 kHz with 50 $\mu$ A amplitude, for 30 seconds across a pair of electrodes, with voltages on 127 electrodes recorded in parallel using the ActiChamp ActiveTwo system with 25 kHz sampling rate. The voltages were demodulated with 2 kHz bandwidth, yielding 1 ms time resolution, and coherent averaging was performed on 60 500 ms trials centered around the time of stimulation. This process was repeated for c. 50 pairs of injection electrodes over the course of 25 minutes to produce a complete data set of c. 6000 voltages. EIT images were reconstructed at each 1ms time point, using the methodology outlined in \cite{Aristovich_2014}.

### Multifrequency 

Multifrequency EIT data was collected as part of clinical trial in collaboration with the Hyper Acute Stroke unit (HASU) at University College London Hospital (UCLH) **ref figure**. Stroke patients were fitted with 32 commercial EEG electrodes (EasyCap, Germany, www.easycap.de) configured using the standard EEG 10-20 \cite{Jasper1958} and 10-10 extension \cite{Oostenveld2001} systems. The electrode application procedure was identical to that used in clinical EEG, with each site cleaned with alcohol and abraded before applying conductive paste. A total of 31 injection pairs were used, with current injected at 17 frequencies between 5 to 2 kHz, for 32 periods at carrier frequencies below 200 Hz, 64 periods between 200 and 1 kHz, and 128 periods above 1 kHz. The amplitude of injected current varied with frequency as per the guidelines in IEC 60601 \cite{IEC}, with the exception of frequencies below 200 Hz which, as as in previous studies \cite{McEwan_2006}, were reduced by half to ensure the current was not perceptible and to avoid saturation of the EEG amplifier. The protocol was repeated three times, taking a total of 20 minutes to complete. 

Data were collected on 10 healthy subjects and 26 patients 

### Impedance Spectrum Measurment

Impedance spectrum measurements have been made with the ScouseTom system \cite{Dowrick_2015}, where low frequency (< 3kHz) impedance measurements were made on healthy (n=112 voltage measurments in 4 rats) and ischaemic (n=56 in 2 rats) rat brain. Impedance data was collected using a 100uA injection through two channels of a 30 electrode array, placed directly on the brain surface. The frequency was increased in 5Hz intervals from 1Hz to 100Hz, 10Hz intervals from 100Hz to 1000Hz and 50Hz intervals between 1000Hz and 3000Hz, with a minimum of 50 periods of the waveform recorded at each frequency. The frequency was swept from 1Hz-3000Hz, 3000Hz-1Hz and with random ordering. The use of an EEG recorder allowed parallel voltage recording at all electrodes, which were averaged together at each frequency. The relative change in impedance, rather than the absolute value, was calculated, by comparing the measured voltages at each frequency.

#Results
##System Characterisation
For resistor phantom measuremnts, the average signal amplitude across 122 measurement combinations and 4235 repeats was 2.66 mV $\pm$ .24 mV standard deviation. The mean noise value for 100 repeats was 0.356 $\mu$V $\pm$ .058 $\mu$V St. Dev., equivalent to 77.5 dB $\pm$ 1.3 dB SNR. As has been found with other EIT systems \cite{oh2007multi}, the long term noise increased, with 0.637 $\mu$V $\pm$ .064 $\mu$V or 72.4 dB $\pm$ 0.66 dB for one hour and 1.522 $\mu$V $\pm$ .205 $\mu$V or 64.9 dB $\pm$ 1.24 dB and four hour recordings. As the short term SNR was unchanged throughout the recording when considering consecutive blocks of 100 measurements figure \ref{SNR}, this decrease in SNR is a result of long term drifts from the baseline voltage. Over the course of the four hour recording the mean change in voltage was 5.61 $\mu$V $\pm$ 1.04 $\mu$V  or 0.21 % $\pm$ 0.04 %. These arise predominantly from temperature changes within the current source, and variations in power supply voltage.

## Frequency response
The mean amplitude decrease, figure \ref{freqresp}, was 1.86 mV V or 21.%  from 20 to 2 kHz for the BioSemi and 0.57 mV or 6.26% for the actiCHamp across the same range. Across the full 20 kHz range the total decrease was 9.15 mV or  99.6 %.  In both cases these frequency responses match those of the anti-aliasing filter within the EEG systems, with cut-offs (-3dB) at 1.7 kHz and 7.5 kHz for the BioSemi and ActiCHamp respectively. Below these cut off frequencies, there was no significant change in mean SNR across frequency, ranging from 66 to 72 dB for the BioSemi and 69 and 75 dB for the ActiChamp.  

##Modes/Experimental Data

Each of the modes of operation previously described have been used in experimental settings. 

### Time difference
During the baseline period before haemorrhage onset, voltages changes of 20.6\(\mu\)V \(\pm\) 51\(\mu\)V (n=7) were observed \ref{FigureStroke}. Over the 10 minute injection period, changes of 20.6mV \(\pm\) 5.4mV occured, with a further increase of 2.2mV \(\pm\) 1.4mV over the remaining measurement time. The time course of the impedance change was consistent with the injection period of the blood into the brain. EIT images were produced using a 0th order Tikhonov algorithm on a 4 million element mesh of a generic rat skull.

### Triggered

### Triggered

Despite the 8-fold increase in bandwidth and consequent noise increase, the performance of the ScouseTom system is comparable to that of previous systems \cite{Oh2011} with 0.37 $\mu$V $\pm$ 0.048 $\mu$V noise across all channels. Significant impedance changes (dV $> 3\sigma$), a single injection pair example in figure \cite{EPDZ}, ranged from 1.20 $\mu$V to 18.7 $\mu$V (mean 3.97 $\mu$V), equivalent to 3.13 to 33.0 (mean 8.86) SNR. EIT reconstructions with this dataset show the onset at 7ms approximately 1 mm below the surface within the primary somatosensory cortex (S1), before expanding to a larger volume until reaching a maximum between 11-12 ms, figure \cite{EPRecon}, then spreading to adjacent areas and finally disappearing at approximately 18 ms. Images obtained previously with a 32 channel system by \citet{Aristovich_2016} with mechanical stimulation of the rat whisker which were found to be in good agreement with established literature, and cross validated with other imaging techniques both in initial onset \cite{armstrong1991thalamo}, and spread of activity \cite{petersen2007functional}. Whilst cross validation was not performed in this study, the literature is equally well established regarding forepaw stimualtion, to which these images are in good agreement \cite{SOMETHING}

### Multifrequency 
**DATA FROM STROKE**

### Impedance Spectrum Measurment

Healthy brain tissue showed a non linear decrease of 15% impedance over 0-250Hz, with ischaemic brain showing a decrease of 7% over the same range, with a more linear slope \ref{FigureSweep}. Above 250Hz, the impedance of both tissue types decreased at the same rate.


