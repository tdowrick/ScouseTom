#Methods
##System Characterisation
Resistor phantom measurements were carried out in order to assess the noise and drift characteristics of the system. The 32 channel Cardiff phantom \cite{griffiths1995cole} was used, configured to a purely resistive load.  Data was collected using the BioSemi EEG system, in a configuration similar to that used during recordings on the human scalp: with current injected at 2 kHz and 100 $\mu$ A, for 100 ms per measurement, over the course of four hours. The noise, defined as the standard deviation, was considered across three time intervals: 100 repeats (approximately five minutes) representing a typical short term measurement, and one and four hours. These longer recordings replicate the use of the system both in Triggered mode, as well as long term monitoring applications \cite{fu2014use} \cite{some lung one}.


## Frequency response

The frequency response was determined using two EEG systems, through measurements on a 32 channel resistive phantom with a current of 100 $\mu$ A. A single measurement was averaged across 32 periods for frequencies below 200 Hz and 64 cycles above, with a total of 64 measurement combinations and 10 repeats. Data was collected over a range 20 Hz to 2 kHz, for the BioSemi system and 20 to 20 kHz for the ActiChamp system, and the results normalised to the lowest frequency.  Ideally with a purely resistive test object, no change in voltage should be seen.

##Modes/Experimental Data

Each of the modes of operation previously described have been used in experimental settings. 

### Time difference
'Standard' time difference EIT data was collected for imaging stroke in a rat model \cite{Dowrick_2016} \ref{FigureStroke}. Using 100\( \mu \)A at 2kHz and ~60 injection pairs, a frame of EIT data was recorded every minute, over 30 minutes. A haemorrhage model was triggered at the 10 minute mark, which was expected to cause a net impedance decrease.

### Triggered

The ScouseTom system was utilised in measurements of evoked activity in the rat somatosensory cortex, following electrical stimulation of the forepaw. The method used closely follows that detailed in \cite{Aristovich_2016} \cite{Vongerichten_2016}, with an increase in the number of electrodes, from 32 on a single hemisphere to 128 with 64 on each hemisphere. The stimuli delivered were 10 mA pulses 1 ms duration at a rate of 2 Hz, triggered by the ScouseTom controller.

Current was injected at 1.7 kHz with 50 $\mu$A amplitude, for 30 seconds across a single pair of electrodes and voltages on 127 electrodes were recorded in parallel using the ActiChamp ActiveTwo system with 25 kHz sampling rate. Coherent averaging was performed on 60 repeated stimuli, and demodulation was performed with 2 kHz bandwidth, yielding 1 ms time resolution. 

### Multifrequency 

Multifrequency EIT data was collected as part of clinical trial in collaboration with the Hyper Acute Stroke unit (HASU) at University College London Hospital (UCLH) **ref figure**. Stroke patients were fitted with 32 EEG electrodes **ref easycap**, and **x** injection pairs were used, with duration **y seconds**. Data was collected over a 30 minute period, at **x** frequencies between **y** and **zHz**, with amplitude **zmA**.

### Characterisation

Impedance spectrum measurements have been made with the ScouseTom system \cite{Dowrick_2015}, where low frequency (< 3kHz) impedance measurements were made on healthy and ischaemic rat brain. Impedance data was collected using a 100uA injection through two channels of a 30 electrode array, placed directly on the brain surface. The frequency was increased in 5Hz intervals from 1Hz to 100Hz, 10Hz intervals from 100Hz to 1000Hz and 50Hz intervals between 1000Hz and 3000Hz, with a minimum of 50 periods of the waveform recorded at each frequency. The frequency was swept from 1Hz-3000Hz, 3000Hz-1Hz and with random ordering. The use of an EEG recorder allowed parallel voltage recording at all electrodes, which were averaged together at each frequency.

#Results
##System Characterisation
For resistor phantom measuremnts, the average signal amplitude across 122 measurement combinations and 4235 repeats was 2.66 mV $\pm$ .24 mV standard deviation. The mean noise value for 100 repeats was 0.356 $\mu$V $\pm$ .058 $\mu$V St. Dev., equivalent to 77.5 dB $\pm$ 1.3 dB SNR. As has been found with other EIT systems \cite{oh2007multi}, the long term noise increased, with 0.637 $\mu$V $\pm$ .064 $\mu$V or 72.4 dB $\pm$ 0.66 dB for one hour and 1.522 $\mu$V $\pm$ .205 $\mu$V or 64.9 dB $\pm$ 1.24 dB and four hour recordings. As the short term SNR was unchanged throughout the recording when considering consecutive blocks of 100 measurements \ref{SNR}, this decrease in SNR is a result of long term drifts from the baseline voltage. Over the course of the four hour recording the mean change in voltage was 5.61 $\mu$V $\pm$ 1.04 $\mu$V  or 0.21 % $\pm$ 0.04 %. These arise predominantly from temperature changes within the current source, and variations in power supply voltage.

## Frequency response
The mean amplitude decrease, figure \ref{freqresp} was 1.86 $uv$ V or 21.% for the BioSemi, **1.86 $uv$ V or 21.%** for the actiCHamp. In both cases these frequency responses match those of the anti-aliasing filter within the EEG systems, with cut-offs at 1.7 kHz and **SOMETHING** kHz for the BioSemi and actiCHamp. Below the cut off frequencies, there was no significant change in SNR across frequency, ranging from 66 to 72 dB for the BioSemi. 

##Modes/Experimental Data

Each of the modes of operation previously described have been used in experimental settings. 

### Time difference - NEED MORE INFO HERE NOISE ETC
**Tom to put in more values here from other paper** voltage changes up to 20mV were observed.

### Triggered

Despite the 8-fold increase in bandwidth and consequent noise increase, the performance of the ScouseTom system is comparable to that of previous systems \cite{Oh2011} with 0.37 $\mu$V $\pm$ 0.048 $\mu$V noise across all channels. Significant impedance changes (dV $> 3\sigma$) , figure \ref{EP_DZ}, ranged from 1.20 $\mu$V to 18.7 $\mu$V (mean 3.97 $\mu$V), equivalent to 3.13 to 33.0 (mean 8.86) SNR. 

### Multifrequency 
**DATA FROM STROKE**

### Characterisation

Data was calculated ate each frequency \ref{FigureSweep}. **TOM TO ADD MORE**

###1 figure/pane for each 'mode':
* convential EIT mode - Tanks \ref{nntankrec} , Rat stroke, Human Stroke (no images)
* Triggered - EPs rat cortex (mayo), Epilepsy Anna V, VEPS Anna WW
* MF - Rat Stroke, Nir Stroke, Tank (not yet)
* Characterisation - Freq response isch, Mayo freq ep
* Rat stroke - time difference data/some images maybe \ref{FigureA} \ref{dV}
* Human stroke - time difference/multi frequency
* Tank/phantom - images
* Nerve - EIT & Action potential
* Epilepsy -EIT & EEG
* Frequency response


