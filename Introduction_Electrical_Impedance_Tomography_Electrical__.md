#Introduction

## Electrical Impedance Tomography
Electrical Imepdance Tomography (EIT) is a medical imaging technique which reconstructs the internal conductivity of an object from boundary measurements. Existing clinical uses of EIT include imaging the lung \cite{Frerichs_2000}, liver \cite{YOU_2009} and breast \cite{Halter}, and a number of EIT systems are now commercially available. EIT has also been proposed for imaging in peripheral nerves and in a number of applications in the brain, including epilepsy \cite{Vongerichten_2016}, \cite{Fabrizi_2006}, acute stroke \cite{Dowrick_2016}, traumatic brain injury and evoked potentials \cite{Aristovich_2016}. The ideal hardware requirements for these applications are not yet known and existing EIT systems, typically designed for imaging the organs of the torso, do not offer all of the capabilities required to identify them.

## EIT Hardware

A typical EIT system consists of a current source, voltage measurement unit, electrode array and some form of control/switching circuitry for automating the measurement process. A sinusoidal current of a defined amplitude and frequency is injected through a pair of electrodes, with voltages measured at all electrodes. This process can be repeated for a number of different pairs of electrodes, producing a set of voltage measurements which can be used to reconstruct a conductivity profile of the target object. Voltages recordings can be performed either serially, or in parallel on all electrodes. 
Existing EIT systems include the KHU \cite{Hun_Wi_2014} (16-64 electrodes, parallel voltage record, multiple pair injection, 11Hz-500kHz, 100 frames/s), fEITER \cite{McCann_2011} (32 electrodes, parallel record, single pair injection at 10 kHz, 100 frames/s), Dartmouth EIT System \cite{Halter} (64 electrodes, 10kHz-1MHz, 100 frames/s) and Swisstom Pioneer Set (32 electrodes, single pair injection at 50 kHz, 50 frames/s).

## Motivation

The optimal measurement paradigms for fast neural EIT and EIT of the head have not yet been established and different experiments can have different requirement \ref{table_requirements}. As such any EIT system for use in these cases should be as versatile as possible, to allow for a range of experimental methods to be investigated. The motivation behind this work was to develop an EIT system which allows for maximum experimental flexibility, satisfying the following criteria:

- Arbitrary control over current amplitude, up to 10mA, and frequency, up to 20kHz. The current levels required for EIT can vary from tens of microamps, for epicortical recordings in rats, to several milliamps when using human scalp electrodes.  Data collection at multiple frequencies can be used for frequency difference EIT and also for characterising the frequency response of a particular tissue or object.
- Parallel recording of all voltages for processing of data 'offline'. It is often beneficial to be able to extract additional signals, such as EEG/ECoG, from the recorded data, alongisde the EIT signal. In order to acheive this, raw voltage data should be recorded by the measurment system, on which application specific data and signal processing can be carried out.
- Noise, frame rate and performance characeristics comparable to existing EIT systems.
- Variable electrode count. EIT experiments typically utilise between 16 and 128 electrodes, dependent on the application.
- Ability to synchronise injection/recording with external triggers (whisker stiumlation, visual, auditory).
- Reconfigurable modes of operation. The system should be as flexible as possible, to allow for new functionality to be introduced as a later date, if additional requirments or experimental methods are identified. Ideally, this should be acheiveable through software/firmware changes only.
- Easily reproducible. Design and construction of a bespoke EIT system can take several months. A system which can be easily replicated using a mixture of off the shelf equipment, alongside open source software and hardware designs, will significantly reduce the workload and allow new systems to be assembled within weeks.


While each of the existing EIT system previously discussed are able to implement some of these requirements, none meet all of them, particularly that of simultaneous EEG recording and fine control over current amplitude and frequency.
