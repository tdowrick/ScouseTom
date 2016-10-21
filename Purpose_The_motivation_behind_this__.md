## Purpose

The motivation behind this work was to develop an EIT system with the maximum flexiblity, such that it could be applied in a range of experimental settings. The following criteria were established:

- Arbitrary control over current amplitude, up to 10mA and frequency in the kHz range. The current levels required for EIT can vary from tens of microamps, for epicortical recordings in rats \cite{Oh2011}, to several milliamps when using human scalp electrodes \cite{tidswell2001three}.  Data collection at multiple frequencies can be used for frequency difference EIT and also for characterising the frequency response of a particular tissue or object.
- Parallel recording of all voltages for processing of data 'offline'. It is often beneficial to be able to extract additional signals, such as EEG/ECoG, from the recorded data, alongisde the EIT signal. In order to achieve this, raw voltage data should be recorded by the measurement system, on which application specific data and signal processing can be carried out.
- Noise, frame rate and performance characeristics comparable to existing EIT systems. Resistance changes by ~0.1% for EIT recording of fast neural activity related to neuronal depolarization. This requires stable current injection, <0.1% noise, and voltage recording with accuracy of ~100nV.
- Variable electrode count. EIT experiments typically utilise between 16 and 128 electrodes, dependent on the application.
- Ability to synchronise injection/recording with external triggers (whisker stimulation, visual, auditory). The phase of injected current should be randomised with respect to the stimulation, to minimise the phase related artefacts in EP recordings \cite{Aristovich_2015}
- Reconfigurable modes of operation. The system should be as versatile as possible, to allow for new functionality to be introduced as a later date, if additional requirments or experimental methods are identified. Ideally, this should be acheiveable through software/firmware changes only.
- Easily reproducible. Design and construction of a bespoke EIT system can take several months and existing publications on EIT systems typically lack enough detail to allow replication. A system which can be easily replicated using a mixture of off the shelf equipment, alongside open source software and hardware designs, will significantly reduce the workload and allow new systems to be assembled in a matter of weeks.


While each of the existing EIT system previously discussed are able to implement some of these requirements, none meet all of them.