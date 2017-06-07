# Tyler Hovanec

[Home](Home.md) | [Professional Experience](ProfessionalExperience.md) | [Education](Education.md) | [Projects](Projects.md)
--------------- | ---------------------------------------------------- | ------------------------- | ----------------------

# Innovar Software and Electrical Engineering Internship 2015-2016

## Position Description

**Department:** Amazon Classification and Catalog Selection Systems  
**Team:** Model Studio Classification Platform  
**Title:** Software and Electrical Engineering Intern  
**Project:** Catalog Item Classification Debug Tool

## Company Background

Innovar Systems Ltd. (Innovar) focuses on specialized industrial automation with tracibility as a primary focus. Traceability means a lot of things; but essentially, given a serial number one can determine which workers, machines, etc. made which component on what day. Now companies can do narrower recalls, compare machine and worker outputs, and view global component calibration or pass/fail statistics for an entire line or single machine.

## Projects

### Electrical Hardware Testing & Verification

Being a relatively small company, everyone wears a lot of hats and I was no exception. Testing and verifying machines after assembly was both a huge task and what held up products from shipping more than anything else.

I tested and verified various large circuit boards and HMI boxes. Testing the individual boards before they were used in assembly was important because the boards were custom made, stuffed with components in house, then placed into a machine. It costs a small amount to test boards before machine assembly because it limits failures to only 1 board and minimizes rework and reassembly time.
 
Testing could involve:
* I/O Verification
* Programming microcontrollers or FPGAs
* Checking signal test points

### Automated Circuit Breaker Calibration Machine

After doing well testing smaller components and sub systems I was assigned a complete machine to test and deliver to the customer.

This was the first ever of this version of this machine so a significant amount of software needed to be written and changed for the new machine. The software was mostly adapted from a core software package and from a similar machine's software.

My To Do List to Deliver to the Customer:
* Update HMI UI (C# + .NET) for new procedures and screens this machine required
* Update microcontroller program to account for new hardware.
* I/O Verification on PLCs, microcontrollers, and 7 HMI boxes
* Electrical verification on high voltage components

Machine Description:
* Concurrently test and calibrate 7 three phase electrical circuit breakers
* Calibrate 3-phase breakers to greater than 95% accuracy
* Deliver up to 700 amps at each of the 7 current sources
* Distributed HMI program across 7 HMI boxes (1 master and 6 slaves)
* Distributed microcontroller program (1 master and 6 slaves)
* 1 Data aggregation device for metrics and traceability

This is no trivial machine or task. There are 15 devices communicating over Ethernet to deliver a lot of electrical current very accurately to multiple breakers concurrently all while aggregating data metrics on serial numbers, calibration details, fixture pass/fail rates, number of calibration passes required, and more.   

### HMI Serial Barcode Scanner Configuration Tool

Following delivery of the automated circuit breaker, I was very familiar with the base HMI application; so I was assigned a project to add a feature to it.

One of the tasks that needs done during testing and verification is configuration. This includes configuring some 40 different barcode scanner parameters to optimal values which are not known in advance. These values used to be hardcoded and would required a recompilation and reboot (long process with Windows CE). This process can easily become very time consuming on a machine with a new scanner placement or new barcode type.
 
Features of my addition:
* New barcode configuration screen for multiple scanners and types
* XML based configuration file to store scanner(s) settings
* Saves up to an hour of developer time during machine configuration

## Technologies

**Languages Used:**
* C#
* .NET Compact Framework
* C
* XML
* Batch Script

**Technologies Used:**
* Windows CE
* Visual Studio
* RS 232 Serial Interface
* 2D & 1D Barcode Scanners
* Atmel Microprocessors
* Atmel AVR Studio
* Alterra Quartus
* Multimeter
* Oscilloscope
* Electrical & Mechanical Hardware Troubleshooting