#System Design

The ScouseTom EIT system consists of a current source (Keithley 6221) and commercial EEG amplifier, alongside custom switching/control circuitry and software. Time and frequency difference EIT data can be collected, at frequencies between 10Hz and 20kHz, with a frame rate > 100 per second achievable.

## Current source

The Keithley 6221 current source is able to produce stable, low noise AC currents in the range 2pA - 100mA, up to a frequency of 100kHz; supports external triggering and phase marking; and is controllable via serial, USB and Ethernet connections.


## Controller and Switch network - TO DO JAMES

The system controller is based upon the Arduino development platform (*ref*), specifically the Arduino Due, and two bespoke PCBs: a controller board or "shield" and a switch network board. The controller shield contains the additional circuitry required for isolating the communication with other components of the system, namely RS232 and trigger-link connections with the current source, TTL with the EEG systems, and SPI connection to the switch networks. Due to the modular nature of the design and the variation of use cases, each connection was separately isolated from the mains to ensure correct isolation regardless of experimental setup.

The current source is programmed via RS232 by the controller, with external triggering and zero-phase marker signals transmitted via a trigger-link cable. This enables the phase of the injected current to be reset upon switching, or shorter injections to be retriggered by an external pulse. Following the suggestions in \cite{Aristovich_2015} the stimulation triggers used in EP studies are randomised with respect to the injected current based on the phase marker signals sent by the Keithley 6221. Alongside the TTL triggers, a simultaneous stimulation voltage with a programmable range of 3 to 18V can be sent.


The switch networks comprise two individual series of daisy chained ADG714 CMOS switches (*Analog Devices ref*), one each for the source and sink connections from the current source. The switch networks themselves can be daisy chained together, thus enabling current injection between any two electrodes from a total of 128. The switchboard is powered via lithium-ion polymer battery, and communicates with the controller through a digitally isolated SPI bus. The possible time between switching electrode injection pairs ranges from 100 uS to approximately 70 minutes for 128 channels, which is more than sufficient to meet the frame rate requirements all use cases. 



controller - needed to be isolated from mains, had to switch quickly so hardware sol. triggers recorded via EEG system digital inputs. phase marker stuff

triggers - control over phase/freq/ampltidue etc. stim pulses variable time/voltage/number



## Voltage recording - TO FINISH
The requirements for voltage recording are parallel data collection, low noise and the ability to save data for offline processing. EEG amplifiers offer an effective off the shelf solution and a number of high performance systems are available \ref{table_eeg}.

## Electrode Connectors - TO DO

DSUB used but often Custom connectors/PCBS required to connect system to common electrode interfaces or our own one in case of rat/nerve


## Controller software - TO DO

ASrduino - ubiquitous and not platform specific, portable to other devices
Serial interface - all commands though this, current in matlab, but could be ported to any language.
