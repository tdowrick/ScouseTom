## Controller and Switch network

The system controller is based upon the Arduino development platform (*ref*), specifically the Arduino Due, and two bespoke PCBs: a controller board or "shield" (*ref in figure*) and a switch network board (*ref in figure*). The controller shield contains the additional circuitry required for isolating the communication with other components of the system, namely RS232 and trigger-link connections with the current source, TTL with the EEG systems, and SPI connection to the switch networks. Due to the modular nature of the design and the variation of use cases, each connection was separately isolated from the mains to ensure correct isolation regardless of experimental setup.

The current source is programmed via RS232 by the controller, with external triggering and zero-phase marker signals transmitted via a trigger-link cable. This enables the phase of the injected current to be reset upon switching, or shorter injections to be retriggered by an external pulse. Following the suggestions in \cite{Aristovich_2015} the variable pulse width stimulation triggers used in EP studies are randomised with respect to the injected current based on the phase marker signals sent by the Keithley 6221. Alongside the TTL triggers, a simultaneous stimulation pulse with a programmable range of 3 to 18V can be sent for direct electrical stimulation.

Coded reference pulses from the controller are recorded by the EEG system and uses as reference during data processing. Pulses are sent to indicate the start and stop of current injection, the switching of electrode pairs, changing of injected frequency, stimulation triggers, and the out-of-compliance status of the current source. 

The switch networks comprise two individual series of daisy chained ADG714 CMOS switches (*Analog Devices ref*), one each for the source and sink connections from the current source. The switch networks themselves can be daisy chained together, thus enabling current injection between any two electrodes from a total of 128. The switchboard is powered via lithium-ion polymer battery, and communicates with the controller through a digitally isolated SPI bus. The possible time between switching electrode injection pairs ranges from 100 uS to approximately 70 minutes for 128 channels, which is more than sufficient to meet the frame rate requirements all use cases. 

## Controller software

Aside from its ubiquity and open source, the additional benefit of basing the controller on the Arduino platform is that it is not hardware specific. Thus porting the software to another device with different architecture is comparatively simple. Currently, the PC software for serial communication with the controller is written in Matlab (*matlab ref*), but the commands can be easily replicated in another language.

## Data processing software  - to do
MATLAB - select bandwidth, averaging etc
