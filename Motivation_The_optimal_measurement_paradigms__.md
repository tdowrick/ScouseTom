## Motivation

The optimal measurement paradigms for fast neural EIT and EIT of the head have not yet been established and different experiments can have different requirements \ref{table_requirements}. As such any EIT system for use in these cases should be as versatile as possible, to allow for a range of experimental methods to be investigated. The motivation behind this work was to develop an EIT system which allows for maximum experimental flexibility, satisfying the following criteria:

- Arbitrary control over current amplitude, up to 10mA, and frequency, in the kHz range. The current levels required for EIT can vary from tens of microamps, for epicortical recordings in rats, to several milliamps when using human scalp electrodes.  Data collection at multiple frequencies can be used for frequency difference EIT and also for characterising the frequency response of a particular tissue or object.
- Parallel recording of all voltages for processing of data 'offline'. It is often beneficial to be able to extract additional signals, such as EEG/ECoG, from the recorded data, alongisde the EIT signal. In order to acheive this, raw voltage data should be recorded by the measurment system, on which application specific data and signal processing can be carried out.
- Noise, frame rate and performance characeristics comparable to existing EIT systems.
- Variable electrode count. EIT experiments typically utilise between 16 and 128 electrodes, dependent on the application.
- Ability to synchronise injection/recording with external triggers (whisker stiumlation, visual, auditory). The phase of injected current should be randomised with respect to the stimulation, to minimise the phase related artefacts in EP recordings \cite{Aristovich_2015}
- Reconfigurable modes of operation. The system should be as flexible as possible, to allow for new functionality to be introduced as a later date, if additional requirments or experimental methods are identified. Ideally, this should be acheiveable through software/firmware changes only.
- Easily reproducible. Design and construction of a bespoke EIT system can take several months. A system which can be easily replicated using a mixture of off the shelf equipment, alongside open source software and hardware designs, will significantly reduce the workload and allow new systems to be assembled in a matter of weeks.


While each of the existing EIT system previously discussed are able to implement some of these requirements, none meet all of them.
