## Schematic and simulation OF CMOS INVERTER,NOR AND NAND GATE USING CADENCE virtuoso
## AIM:
  to schematic and simulate inverter using CADENCE virtuoso.
## APPARATUS REQUIRED:
CADENCE VIRTUOSO
## PROCEDURE:
## Procedure for Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
   i)	tcsh
   ii)	source /home/install/cshrc
   iii)	virtuoso 
## Procedure for Schematic simulation using Cadence
1.	Now two windows must open i)virtuoso/command interpreter window 
   ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
   i)	Create a New Library
   ii)	Create Schematic Cell view.
   iii)	Create the Symbol for schematic Cell view.
   iv)	Create the test Cell view.
    v)	Analog simulation by spectre
## Procedure for Creating New Library.
a)	File –New – Library
b)	Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing technology library, Click OK
c)	Attach the library to the technology library gpdk045.Click OK
## Create Schematic Cell view.
a)	Go to 1st window i.e virtuoso(CIW)
b)	File-New-Cell view
c)	Setup the new file form, Library: Select the one you a created. Cell : Give the experiment name Ex: Inverter View: Schematic
d)	Type: Schematic press OK
e)	Add the required components from the libraries and make the connections.
f)	Go to instance fixed menu or use shortcut key “I” from keypad to go instances Click on browse. This opens the library browser ow select the appropriate library for components like Gpdk045,nmos, pmos
g)	Analog library	Vdd, Gnd, Vcc, Vpulse, Vsin
h)	Make the connections by using fixed narrow wire key
i)	Click Check and Save button

## Creating the Symbol for schematic Cell view
a.	In the schematic window, execute
Crate – Cell view – From Cell view
The cell view from cell view window appears
Check Lib Name, Cell Name, From View name must be schematic Press ok
b.	Now Symbol generation form appears. Click Ok If No changes required
c.	A new window with with default symbol is created.
d.	Edit the symbol if you want to give actual symbol shape else continue.
i.	Execute Create-Cell view-from cell view
ii.	Library Name and Cell Name must be same which you have used for schematic. Press OK
iii.	Check for the position of pin side.Prss OK
iv.	Edit for the shape by Create-Shape-Choose required options to edit.

## Creating the new test cell view
a)	Go to CIW window, Execute File-New-Cell view
b)	Setup the new file form
Library: Select the one you a created.
Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
View: Schematic
Type: Schematic  press OK
Analog simulation by SPECTRE.
a.	In test cell view window
b.	Launch – ADE L(Analog Design Environment)
c.	Execute Setup—Simulation/directory/Host A new window opens
d.	Set the simulation window to spectre and click ok
e.	Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and section type as stat then press OK.
f.	Execute Analysis – Choose. A window opens.
g.	Select the type and set the specifications and press OK
h.	Execute Output s—to be plotted – Select on Schematic
i.	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
j.	Execute Simulation -- Net list and Run

## INVERTER:

![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/e7278808-2830-4f7d-877f-1d3205fa6490)

![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/df72ec90-5964-4f7e-a939-2c8740fe5d5c)

## Specifications: 
Vpulse 	V1 = 0	Vdc	= 1
V2 = 1
td = 0,tr=tf=1 n, ton= 100n ,T=200n
## OUTPUT:
## Simulation Settings
## Setup for transient analysis:
1.	Stop time =400n
## Setup for D.C analysis
1.	Component to be selected in schematic is	for d.c analysis
2.	Start = -1 Stop = 1 resp.

## Transient Analysis:

![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/cb9ad5bb-1e37-4e6c-a6fb-007db33bd416)

 ## DC Analysis:
![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/2e8400be-435c-47d7-991b-578f07188141)
## 2 INPUT NAND:
![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/123f6896-ae89-4201-be01-6f4d977f6a67)
![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/d4c7cd0b-4a5f-4421-860d-e09fe20f403e)
## Specifications:
    Vpulse A V1 = 0, V2 = 1,Vpulse B V1 = 0, V2 = 1
    Vdc = 1
    For Vpulse A td = 0,tr = tf = 1 n, ton = 200n ,T = 100n
    For Vpulse B td = 0,tr = tf = 1 n, ton = 100n ,T = 50n

## OUTPUT: Simulation Settings
## Setup for transient analysis:
    1.Stop time =400n
    
![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/388f55f0-4d89-45a6-bc28-a6c063da8a4e)

## 2 INPUT NOR:

![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/ecbcceee-4c23-47f4-acc3-9921796283b1)

![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/a4c74062-9c7e-4b56-b5d5-3186e06a4172)

## Specifications:     V
    Vpulse A V1 = 0, V2 = 1,Vpulse B V1 = 0, V2 = 1
    Vdc = 1
    For Vpulse A td = 0,tr = tf = 1 n, ton = 200n ,T = 100n
    For Vpulse B td = 0,tr = tf = 1 n, ton = 100n ,T = 50n

## OUTPUT: Simulation Settings
## Setup for transient analysis:
    1.Stop time =400n

![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/66394093-3df1-46a6-8290-5f0d1aa308f4)

## RESULT:
The schematic and simulate inverter using CADENCE is done and verified successfully.



