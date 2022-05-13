# INTRODUCTION

Today’s car wipers are manual systems that work on the
principle of manual switching. So here we propose an automatic wiper system that automatically switches ON on
detecting rain and stops when the rain stops. Our project
brings forward this system to automate the wiper system
not need manual intervention.

For this purpose, we use a
rain sensor along with a microcontroller to drive the wiper
motor. Our system uses a rain sensor to detect rain, this
signal is then processed by a microcontroller to take the
desired action.

The rain sensor works on the principle of
using water for completing its circuit, so when rain falls
on it, the circuit gets completed and sends out a signal to
the microcontroller. The microcontroller now processes this
data and controls the motor.

# WORKING

* The RED LED is considered for the ACC position. Once the push button is pressed for 2 seconds, the RED LED keeps continuously glowing until the stop of the engine signifying the engine condition to be turned ON.
* On press of the user input push button, the other three Blue, Green and Orange LEDs come ON one at a time with the set frequency. The frequency changes on every alternate key press, 3 frequency levels with 1, 4 and 8 Hz.
* The LED glow pattern stops on the 4th press; the wiper action starts with the next press.
* If the push button is pressed for 2 seconds continuously, the RED light goes off and the pattern stops bringing it to default position which signifies the engine is turned OFF.

# REQUIREMENTS FOR THE PROJECT

## STM32Cube IDE

* STM32Cube software ecosystem. STM32CubeIDE is an advanced C/C++ development platform with peripheral configuration, code generation, code compilation, and debug features for STM32 microcontrollers and microprocessors. It is based on the Eclipse®/CDT™ framework and GCC toolchain for the development, and GDB for the debugging. It allows the integration of the hundreds of existing plugins that complete the features of the Eclipse® IDE

## Xpack Packages

## Windows Build Tools

* The xPack Windows Build Tools is a standalone Windows binary distribution of GNU make and a few of other tools required by the Eclipse Embedded CDT (formerly GNU MCU/ARM Eclipse) project, but the binaries can also be used in generic build environments.

## OpenOCD

* Open On-Chip Debugger (OpenOCD) is a free, open-source project that aims to provide debugging, in-system programming, and boundary scan using a debug adapter. The adapter is a hardware module that provides the right signals for the target to understand.

## QEMU

The xPack QEMU Arm is a standalone cross-platform binary distribution of QEMU, with several extensions for Arm Cortex-M devices.

# COMPONENTS USED IN PROJECT

## STM32F407G-DISC1

STM32F407 series of microcontrollers are high-performance MCUs designed for medical, industrial and consumer applications. It is based on ARM Cortex-M4 and offers up to 168MHz. The STM32F407VGT6 is the onboard chip which comes in a 100-pin LQFP package.

The STM32F407G-DISC1 is a Discovery Kit allows users to easily develop applications with the STM32F407 high performance microcontrollers with ARM cortex-M4 32-bit core. It includes everything required either for beginners or for experienced users to get quickly started. Based on the STM32F407VGT6, it includes an ST-LINK/V2 or ST-LINK/V2-A embedded debug tool, two ST MEMS digital accelerometers, a digital microphone, one audio DAC with integrated class D speaker driver, LEDs and push buttons and an USB OTG micro-AB connector.

## Features Of STM32F407G

* Flash memory of up to 1 megabyte.
* OTP memory of 512 bytes.
* Compact Flash, SRAM, PSRAM, NOR, and NAND memories are supported by this flexible static memory controller.
* Sleep, Stop, and Standby modes are low-power modes.
* 16-stream DMA controller with FIFOs and burst support for general-purpose DMA.
* Up to 54 Mbytes/s 8- to 14-bit parallel camera interface.
* Generator of true random numbers.
* Hardware calendar, CRC calculating unit, 96-bit unique ID RTC, subsecond accuracy.

# 4 W'S

## WHAT IS WIPER SYSTEM

Windscreen wipers are necessary for maintaining sufficient view for the driver, especially in modern high-speed cars.

## WHY WIPER SYSTEM

To keep the windscreen clean enough to give adequate view at all times.

## WHEN SHOULD USE WIPER SYSTEM

The windshield wipers remove rain and snow from the windshield, while the headlights improve visibility at night.

## WHO DISCOVERED WIPER SYSTEM

Mark Anderson invented on 1902

# SWOT Analysis

## Strength

* Visibility
* The wiper does not stop in the middle of the window during drive.
* Safety

## Weakness

* High cost
* Not automatic

## Opportunities

* Rain sensing and automatic operation can be implemented as further enhancement.

## Threats

* Once the board repaired cannot be replaced quickly

# REQUIREMENTS

## High Level Requirements

|  ID  |   Description   |  Status  |
|------|-----------------|----------|
| HR_01| ACC Mode Operation| Implemented|
| HR_02|Wiper ON| Implemented|
| HR_03|Wiper Speed Change|Implemented|
|HR_04|Wiper OFF|Implemented|


## Low Level Reuirements

| ID	| Description	| Operation	|Status |
|-----|-------------|-----------|-------|
|LR_01|	Button pressed once for 2 secs|	Red LED ON	|Implemented|
|LR_02|	Button pressed second time|	1 Hz speed - Blue, Green Orange alternative|Implemented|
|LR_03|	Button pressed third time|	4 Hz speed - Blue, Green Orange alternative	|Implemented|
|LR_04|	Button pressed fourth time|	8 Hz speed - Blue, Green Orange alternative|	Implemented|
|LR_05|Button pressed again for two seconds|	Turn Off all LEDs|	Implemented|
