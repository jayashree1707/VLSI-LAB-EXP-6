## ANALOG DESIGN OF INVERTER,NOR AND NAND GATE USING VIRTUOSO
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
![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/46d1926f-597d-4aee-9bb8-cd816072c15a)
![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/99a7bffd-dbfe-4f53-9ff7-34216f329cc2)
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
![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/aad81ae9-ea5e-459b-ae73-c9c366433d58)
 ## DC Analysis:
![image](https://github.com/jayashree1707/VLSI-LAB-EXP-6/assets/160314881/cfd6c933-008e-483c-8d59-7a5285d2ca9b)






