Demonstration algorithm for PiFace Digital on Raspberry Pi 
==========================================================

This folder contains the source files for the demonstration project on using the 
REX Control System and the Raspberry Pi minicomputer with 
the PiFace Digital extension board.

The four pushbuttons of the PiFace Digital are used for demonstration of simple 
algorithms in the REX Control System:

- The first push-button controls the first onboard relay directly. The signal 
just needs to be inverted due to the inverted logic of the inputs and outputs of 
the PiFace Digital board. 
- The second push-button toggles the state of the second onboard relay. Edges in 
the input signal are detected, which toggle the state of an RS flip-flop function 
block.
- The third push-button blinks the third output by feeding the binary signal 
generator into it.
- The fourth push-button triggers a timer, which activates the fourth output for 
a predefined period.

The timer can also get triggered by a "virtual button" (the MP_START function 
block).

The remaining outputs of PiFace Digital are controlled directly by user-defined 
Boolean constants. 

## Prerequisities ##

- RexCore and RPiDrv modules must be installed and running on the Raspberry Pi.
- SPI bus must be enabled on the Raspberry Pi.

## Running the example ##

- The **exec.mdl* file is the project main file, open it with RexDraw.
- Compile and download the project to the target device.

## User interface (HMI) ##
The example is accompanied by a HTML5-based user interface built on the WebBuDi 
framework (Web Buttons and Displays) of the REX Control System. Download it to 
the Raspberry Pi using the RexView diagnostic tool.

## Documentation ##

- [Getting started with REX and Raspberry Pi](http://www.rexcontrols.com/media/DOC/ENGLISH/REX_Getting_Started_RasPi_ENG.pdf)
- [Function blocks of the REX Control System](http://www.rexcontrols.com/media/HTML/DOC/ENGLISH/index.html)
- [Complete documentation of the REX Control System](http://www.rexcontrols.com/documentation-and-support)

## Additional information ##

- Raspberry Pi is a trademark of the [Raspberry Pi Foundation](http://www.raspberrypi.org).
- Visit the [REX Controls company webpage](http://www.rexcontrols.com) 
for more information about the example projects and developing advanced 
automation and control solutions using the REX Control System.