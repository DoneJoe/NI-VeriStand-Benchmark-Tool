## NI VeriStand Benchmark Tool ##

**NI VeriStand Benchmark Tool** redeploys a system definition to a NI Real-Time (RT) target until the highest stable loop rate is found. 

The criteria for a passing configuration includes no additional late counts for 15 seconds after a 15 second warmup period and achieving the requested loop rate within a user defined %.

When run, it prompts you to specify a path on disk with nisysdef files. It will then deploy those configurations over and over at different rates, performing a binary search, to find the highest rate they can successfully run at.

If you have multiple targets in your configuration, it will set all of them to the same rate as it searches.

If AND ONLY IF you are using the provided configuration files, make sure you're using 7831R's as RIO0 and RIO1, and DAQ cards named "Dev1 and Dev2". Else, go to step 2.

The tool will let you know its progress as it goes through the configurations and writes out a report at the end.

### LabVIEW Version ###

LabVIEW 2011

### Built Availability ###

Builds are available [here](http://www.ni.com/example/31441/en/).

### Quality, Limitations ###

The tool was developed in 2010 and used each release of NI VeriStand, thus should be considered mature and well tested. However it CURRENTLY ONLY TESTS IF THE FIRST TARGET IN A SYSDEF FAILED TIMING! Update the Pass Fail Check.vi to change this.

### License ###

*This repository and any materials provided by NI therein are provided AS IS. NI DISCLAIMS ANY AND ALL LIABILITIES FOR AND MAKES NO WARRANTIES, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR  PARTICULAR PURPOSE, OR NON-INFRINGEMENT OF INTELLECTUAL PROPERTY. NI shall have no liability for any direct, indirect, incidental, punitive, special, or consequential damages for your use of the repository or any materials contained therein.*