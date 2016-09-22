#Results
##System Characterisation
For resistor phantom measurements, the average signal amplitude across 122 measurement combinations and 4235 repeats was 2.66 mV $\pm$ .24 mV standard deviation. The mean noise value for 100 repeats was 0.356 $\mu$V $\pm$ .058 $\mu$V St. Dev., equivalent to 77.5 dB $\pm$ 1.3 dB SNR. As has been found with other EIT systems \cite{oh2007multi}, the long term noise increased, with 0.637 $\mu$V $\pm$ .064 $\mu$V or 72.4 dB $\pm$ 0.66 dB for one hour and 1.522 $\mu$V $\pm$ .205 $\mu$V or 64.9 dB $\pm$ 1.24 dB and four hour recordings. As the short term SNR was unchanged throughout the recording when considering consecutive blocks of 100 measurements figure \ref{SNR}, this decrease in SNR is a result of long term drifts from the baseline voltage. Over the course of the four hour recording the mean change in voltage was 5.61 $\mu$V $\pm$ 1.04 $\mu$V or 0.21 % $\pm$ 0.04 %. These arise predominantly from temperature changes within the current source, and variations in power supply voltage.

## Frequency response
The mean amplitude decrease, figure \ref{freqresp}, was 1.86 mV V or 21.%  from 20 to 2 kHz for the BioSemi and 0.57 mV or 6.26% for the actiCHamp across the same range. Across the full 20 kHz range the total decrease was 9.15 mV or  99.6 %.  In both cases these frequency responses match those of the anti-aliasing filter within the EEG systems, with cut-offs (-3dB) at 1.7 kHz and 7.5 kHz for the BioSemi and ActiCHamp respectively. Below these cut off frequencies, there was no significant change in mean SNR across frequency, ranging from 66 to 72 dB for the BioSemi and 69 and 75 dB for the ActiChamp.  

##Experimental Data

Each of the modes of operation previously described have been used in experimental settings. 

### Time difference
During the baseline period before haemorrhage onset, voltages changes of 20.6\(\mu\)V \(\pm\) 51\(\mu\)V (n=7) were observed \ref{FigureStroke}. Over the 10 minute injection period, changes of 20.6mV \(\pm\) 5.4mV occured, with a further increase of 2.2mV \(\pm\) 1.4mV over the remaining measurement time. The time course of the impedance change was consistent with the injection period of the blood into the brain. Previous investigation into data rejection methods for measurements using collected with other EIT systems, suggested removal of up to 30 % of all channels in phantoms were necessary \cite{packham2012comparison}. However, only 10 % of channels were rejected from this dataset using similar criteria, suggesting an improvement in the quality of the data, despite the more complex experimental scenario.

###Scalp Recordings
The mean signal amplitude across all subjects was 5.4 mV $\pm$ 1.97 mV, and the mean drift across the length of the recordings was 15.1 $\mu$V or 0.26 %. The mean noise across all 540 measurements and 60 repeats ranged from 8.55 $\mu$V to 53.9 $\mu$V between patients, with an overall noise of 37.2  $\mu$V $\pm$ 39.0 $\mu$V across all measurements, repeats and subjects. The equivalent SNR was 46.5 dB $\pm$ 4.14 dB, ranging from 41.6 to 56.0 dB between subjects. As with the long term resistor phantom recordings, the drifts across the recordings reduced the equivalent SNR. Additionally, artefacts resulting from subject or electrode movement were present some recordings, further reducing the effective SNR in these cases.  

### Triggered

Despite the 4-fold increase in bandwidth and consequent noise increase, the performance of the ScouseTom system is comparable to that of previous systems \cite{Oh2011} with 0.37 $\mu$V $\pm$ 0.048 $\mu$V noise across all channels. Significant impedance changes (dV $> 3\sigma$), a single injection pair example in figure \ref{EPDZ}, ranged from 1.20 $\mu$V to 18.7 $\mu$V (mean 3.97 $\mu$V), equivalent to 3.13 to 33.0 (mean 8.86) SNR. 

EIT reconstructions with this dataset show the onset at 7ms approximately 1 mm below the surface within the primary somatosensory cortex (S1), before expanding to a larger volume until reaching a maximum between 11-12 ms, figure \ref{EPRecon}, then spreading to adjacent areas and finally disappearing at approximately 18 ms. Images obtained previously with a 32 channel system by \citet{Aristovich_2016} with mechanical stimulation of the rat whisker which were found to be in good agreement with established literature, and cross validated with other imaging techniques both in initial onset \cite{armstrong1991thalamo}, and spread of activity \cite{petersen2007functional}. Whilst cross validation was not performed in this study, the literature is equally well established regarding forepaw stimulation, to which these images are in good agreement \cite{peeters2001comparing} \cite{masamoto2007relationship} \cite{lowe2007small}.

### Multifrequency 

The variation in SNR across frequency, figure \ref{MFSNR}, averaged over all patients, repeats and measurements was not significant, ranging from 44.1 to 45.5 dB.  However, all of the frequencies below 200 Hz, the SNR was 1dB less than subsequent frequencies. These correspond to those with a lower number of sine wave periods averaged per measurement, and suggest the number of averages should be increased in order to obtain a more uniform response across frequency. 

As figure \ref{MFSNR} shows the range of 

The SNR of the longer term recordings also did not demonstrate any frequency dependence, with a mean SNR of 41.6 $\pm$ 7.9 dB, 41.4 $\pm$ 8.25 dB and 40.7 $\pm$ 8.2 dB for 0.2 1.2 and 2 kHz respectively. Similarly the mean change in impedance was 0.74 %, 0.61 % 0.68 %, and was thus largely unchanged across frequency.  


### Impedance Spectrum Measurment

Healthy brain tissue showed a non linear decrease of 15% impedance over 0-250Hz, with ischaemic brain showing a decrease of 7% over the same range, with a more linear slope \ref{FigureSweep}. Above 250Hz, the impedance of both tissue types decreased at the same rate.


