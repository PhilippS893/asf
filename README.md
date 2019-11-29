# USE ASF IN COIMBRA (Edited 20191129)
New functionality was implemented to use:
1. a CedrusResponseBox (RB-730 series)
2. a custom made button box
3. serial trigger collection from the Siemens Prisma scanner and response collection from a 4 button Lumina device.

You need the following parameters to use the abovementioned devices:
1. CedrusResponseBox<br/>
```matlab
  Cfg.responseDevice = 'CEDRUSSERIAL';<br/>
  Cfg.serialPortName = 'your port name';<br/>
  Cfg.responseType = 'buttonDownCedrus';<br/>
  ```
2. Custom built response box<br/>
```matlab
  Cfg.responseDevice = 'CUSTOMPARALLEL';<br/>
```

3. at the Scanner:<br/>
```matlab
  Cfg.synchToScanner = 1;<br/>
  Cfg.synchToScannerPort = 'SCANNERCOIMBRA';<br/>
  Cfg.scannerPortName = 'COM2'; % assign the correct port here if the scanner is not COM2 by default<br/>
  Cfg.responseDevice = 'LUMINACOIMBRA';<br/>
  Cfg.serialPortName = 'COM3';<br/>
  Cfg.responseType = 'buttonDown';<br/>
```

# asf
asf is a tool for presenting visual, auditory, and tactile stimuli in behavioural experiments under Windows, Linux and OSX using the Psychophysics Toolbox www.psychtoolbox.org and Matlab. It provides a framework for connecting with data acquisition devices such as MRI- and MEG/EEG scanners, and with stimulation devices such as TMS and tactile stimulators.

## Introductory Material
ASF is described in 
Schwarzbach, J. (2011). A simple framework (ASF) for behavioral
and neuroimaging experiments based on the psychophysics toolbox for MATLAB. Behav Res 43, 1194-1201. [pdf] (https://github.com/jvschw/asf/blob/master/documentation/Schwarzbach%202011%20BehavResMeth%20ASF.pdf)

## WIKI
https://github.com/jvschw/asf/wiki

## Website
http://jvschw.github.io/asf/

