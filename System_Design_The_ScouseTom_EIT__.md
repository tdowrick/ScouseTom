#System Design

The ScouseTom EIT system consists of a current source (Keithley 6221) and commercial EEG amplifier, alongside custom switching/control circuitry and software. Time and frequency difference EIT data can be collected, at frequencies between 10Hz and 20kHz, with a frame rate > 100 per second achievable.

## Current source

The Keithley 6221 current source is able to produce stable, low noise AC currents in the range 2pA - 100mA, up to a frequency of 100kHz; supports external triggering and phase marking; and  is controllable via serial, USB and Ethernet connections.


## Switch network/control/trigger interface - TO DO

contoller - needed to be isolated from mains, had to switch quickly so hardware sol. triggers recorded via EEG system digital inputs. phase marker stuff

triggers - control over phase/freq/ampltidue etc. stim pulses variable time/voltage/number

sw net - isolated and easily reconfigurable, and daisy chainable. SPI

## Voltage recording - TO FINISH
The requirements for voltage recording are parallel data collection, low noise and the ability to save data for offline processing. EEG amplifiers offer an effective off the shelf solution and a number of high performance systems are available \ref{table_eeg}.

## Electrode Connectors - TO DO

DSUB used but often Custom connectors/PCBS required to connect system to common electrode interfaces or our own one in case of rat/nerve

testing offline

## Controller software - TO DO

ASrduino - ubiquitous and not platform specific, portable to other devices
Serial interface - all commands though this, current in matlab, but could be ported to any language.
