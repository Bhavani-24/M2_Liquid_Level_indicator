# Requirements
## Introduction

Water is a vital but scarce natural resource. To prevent water wastage, this water tank overflow indicator comes in handy. It gives audio as well visual alarm whenever the water tank overflows.Basically automation in systems would help reduce wastage of resources in various ways, one such way for the prevention of wastage of water resource to control the water tanks from overflow. In this automated world, the handling of any kind of devices with comfort is made to be the easiest factor everywhere. Considering this aspect of comfort zones and the prevention of wastage of resources, a design of an automated overflow control circuit unit was proposed. The proposal was designed on the perspective of controlling the flow of water into the tanks automatically.

## Features

> * No water wastage.
> * No power wastage.
> * High quality shock pruf plastic box.
> * Maintenance free.
> * Long life system.

## Components Required

> * Atmega328p - A single-chip microcontroller created by Atmel in the megaAVR family
> * SimulIDE - A simple real time electronic circuit simulator
> * VS Code - Visual Studio Code is a code editor redefined and optimized for building and debugging modern web and cloud applications
> * HD44780-165 Display – This is the display for showing water level
> * LED - A light-emitting diode (LED) is a semiconductor light source that emits light when current flows through it
> * Potentiometer - A potentiometer is a simple mechanical device that provides a varying amount of resistance when its shaft is turned.
> * Resistor - A resistor is a passive two-terminal electrical component that implements electrical resistance as a circuit element
> * Switch - Switches are used to turn ON/OFF devices and to connect different parts of a circuit.

## Detail Requirement

## High level requirements

ID | Description | Status
----|----------- |-------
HLR1 | display level | Implemented
HLR2 | flow water when level low | Implemented
HLR3 | stop water flow when level is reached | Implemented

## Low level requirements

ID | Description | Status
--- | ---------- | ------
LLR1 | if low level switch open before uplevel the water won't flow | Implemented
LLR2 | the system works without errors | Implemented

## Project working

1. The display is used in this circuit which displays the water level and potentiometer is used that provides the varying amount of resistance.
2. The source code this project is available and after running the code, the .hex file and .elf file is created.
3. Build the circuit according to the below diagram
![image](https://user-images.githubusercontent.com/104186419/164953982-b7b48408-5769-42d3-b8dd-bc2a727e6357.png)
4. In simulIDE click on mcu and click on load the firmware, and select .hex file
5. Finally the circuit works
6. The results are seen in the display.

## Applications

1. Can be used in factories
2. commercial complexes
3. apartments
4. home
5. Fuel tank level gauging

## Block Diagram

![image](https://user-images.githubusercontent.com/104186419/164954135-d4ed829a-ff37-46cd-a09f-a6e1f86158ca.png)

## Circuit Diagram

![image](https://user-images.githubusercontent.com/104186419/164954248-b8d33b4c-1bb3-4bbd-9127-a1b620118572.png)

# Test Plan and Output

## High level test plan

Test ID | Description | Exp Input | Exp Output | Actual Output | Status
------- | ----------- | --------- | ---------- | ------------- | ------
H_01 | Display Level Of Water | NA | 0L - 3000L | 700L | Pass
H_02 | LED Glows when both Switches Open | NA | LED Glows | LED Glows | Pass
H_03 | LED OFF when both Switches Closed | NA | LED OFF | LED OFF | Pass

## Low level test plan

Test ID | Description | Exp Input | Exp Output | Actual Output | Status
------- | ----------- | --------- | ---------- | ------------- | ------
L_01 | LED Glows when UCC only open | NA | LED Glows | LED Glows | Pass
L_02 | Level of water varies from 0L - 3000L | NA | varies from 0L - 3000L | varies from 0L-3000L | Pass

































