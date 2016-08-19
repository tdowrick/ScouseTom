#System Design

The ScouseTom EIT system consists of a current source (Keithley 6221), custom switch network & control circuitry, and EEG amplifer (BioSemi/actiCHamp/GTec). Time and frequency difference EIT data can be collected, at frequencies between 10Hz and 20kHz, with a frame rate > 100 per second achievable.

## Current source

The Keithley 6221 current source is able to produce stable, low noise AC currents in the range 2pA - 100mA, up to a frequency of 100kHz; supports external triggering and phase marking; and  is controllable via serial, USB and Ethernet connections. 


## Switch network/control/trigger interface

contoller - needed to be isolated from mains, had to switch quickly so hardware sol. triggers recorded via EEG system digital inputs. phase marker stuff

triggers - control over phase/freq/ampltidue etc. stim pulses variable time/voltage/number 

sw net - isolated and easily reconfigurable, and daisy chainable. SPI

## EEG
An off the shelf solution for voltage recording, in the form of an EEG amplifier, was chosen. A number of systems are available which offer excellent performance.
actichamp system used too - software same use open source libraries. versatiblity in data processing - can collect wide band data, or change after exp.

## Electrode Connectors

DSUB used but often Custom connectors/PCBS required to connect system to common electrode interfaces or our own one in case of rat/nerve

## Controller software

ASrduino - ubiquitous and not platform specific, portable to other devices
Serial interface - all commands though this, current in matlab, but could be ported to any language. 