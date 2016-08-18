#Introduction

## General EIT Intro & Applications (brain/nerve)

## Existing EIT Systems (SwissTom, KHU, Dartmouth, UCL Mk 2.5 etc)

A typical EIT system consists of a current source, voltage measurement unit, electrode array and some form of control/switching circuitry for controlling the measurement process. A sinusoidal current, of a defined amplitude and frequency, is injected through a pair of electrodes, with voltages measured at all electrodes. This process can be repeated for a number of different pairs of electrodes, producing a set of voltage measurements which can be used to reconstruct a conductivity profile of the target object.

## Motivation

The optimal measurement paradigms for fast neural EIT and EIT of the head have not yet been established. As such any EIT system for use in these cases should be as versatile as possible, to allow for a range of experimental methods to be investigated. To allow for maximum flexibility, a new system was designed with the following requirements:

- Arbitrary control over current amplitude, up to 10mA, and frequency, up to 20kHz. The current levels required for EIT can vary from tens of microamps, for epicortical recordings in rats, to several milliamps when using human scalp electrodes.  Data collection at multiple frequencies can be used for frequency difference EIT and also for characterising the frequency response of a particular tissue or object.
- Parallel recording of all voltages for processing of data 'offline'. It is often beneficial to be able to extract additional signals, such as EEG/ECoG, from the recorded data, alongisde the EIT signal. In order to acheive this, raw voltage data should be recorded by the measurment system, on which application specific data and signal processing can be carried out.
- Reconfigurable modes of operation. The system should be as flexible as possible, to allow for new functionality to be introduced as a later date, if additional requirments or experimental methods are identified. Ideally, this should be acheiveable through software/firmware changes only.
- Easily reproducible. Design and construction of a bespoke EIT system can take several months. A system which can be easily replicated using a mixture of off the shelf equipment, alongside open source software and hardware designs, will allow new systems to be deployed within weeks and with minimal effort.

##Syste4m specs
* EEG simultaneous - EEG and software
* Low Freq w/ fine control and optional trigger phase control/ retriggering  - CS
* Versatile sig pro - different experimental paradigms, change post hoc - EEG and software 
* Simple to reconfigure mode of operation - software reconfigurable. elec platinastion, safety study (arb long injections), easy to connect and trigger off different things VEPs etc. OPEN SOURCE CODE - ALL
* Easily reproducable - off the shelf parts, and open source hardware mix. Make a new one in days rather than months of redisgn. Compare cost/time investment to other DIY systems (KHU etc). SwissTom or other purchasable systems dont do what we want  - ALL - only 2 custom PCBs - schematics open source

While each of the existing EIT system previously discussed are able to implement some of these requirements, none meet all of them, particularly that of simultaneous EEG recording and fine control over current amplitude and frequency.
