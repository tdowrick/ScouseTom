## Voltage recording - TO FINISH
The requirements for voltage recording are parallel data collection, low noise and the ability to save data for offline processing. EEG amplifiers offer an effective off the shelf solution and a number of high performance systems are available \ref{table_eeg}. Each system offers a PC GUI, data streaming over TCP/IP and the option to write custom software to interface with the device. The downside of using an EEG amplifier, is that the maximum EIT frequency is limited to tens of kHz, compared to other systems which can operate up to several MHz. For brain EIT, this is not an issue as the frequencies of interest are typically in the kHz range, but it may be an obstacle for certain applications.

## Electrode Connectors - TO DO

DSUB used but often Custom connectors/PCBS required to connect system to common electrode interfaces or our own one in case of rat/nerve


## Controller software - TO DO

ASrduino - ubiquitous and not platform specific, portable to other devices
Serial interface - all commands though this, current in matlab, but could be ported to any language.
