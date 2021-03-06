# ScoreBoardingViz
Visualization of Scoreboarding Algorithm ( Dynamic Scheduling Algorithm)
Scoreboard Simulator Program

Author: Aditya Malshikhare

1. Input 

This program uses an input file called data.in that has a list of MIPS64 instructions.
Example of this is: 

L.D        F2, 0(R1)
ADD.D      F6, F2, F4
MULT.D     F8, F6, F0
L.D        F10, -8(R1)
ADD.D      F12, F10, F4
MULT.D     F14, F12, F10
DADDUI     R1, R1, #-16

2. Logic and Implementation

The program then utilizes a Scoreboard logic and schedules the instructions. The scoreboard
accepts instructions that use Immediate and Offset Addressing Modes and stores the appropriate
values as a part of the Registers associated with a single instructions. The Scoreboard is
able to schedule Unsigned instructions, but it will not maintain proper values for it. It only
handles signed values.

3. Compiling/Running the Program

This program assumes the environment is correctly setup with Java 6 on Windows. Any deviations
in this configuration will require additional setup parameters.

To Compile and Run the Program, change a command prompt to the directory where the source files 
reside. To compile the program, type:

javac *.java

To run the program, place the source file with the filename data.in in the directory of the class
files created from the above compilation process and run with the command:

java Project

If not using Windows, you must first be sure that you setup your
display Variable. 

E.g. Bash: export DISPLAY=myIP:0
     Tcsh: setenv DISPLAY myIP:0

Without a display set, the X windows system will not be able to display the menu of the program.	 
