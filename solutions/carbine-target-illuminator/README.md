# CARBINE TARGET ILLUMINATOR
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-email.png)

## [SOLUTION 1](/solutions/carbine-target-illuminator/carbine-target-illuminator-0.txt)
#### DESCRIPTION
My inital solution was to split the problem into three pieces:
1. Timer to count the length of the radar pulse
2. Mode/State selector that will choose the state based on the pulse length
3. Controller that will send the correct outputs based on the state
#### PARTS
- 2x MC4000 HIGH PERFORMANCE MICROCONTROLLER
- 1x MC6000 HIGH PERFORMANCE MICROCONTROLLER
- 1x DX300 DIGITAL I/O EXPANDER
#### PERFORMANCE
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-0-stats.png)
#### DIAGRAM
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-0.png)


## [SOLUTION 2](/solutions/carbine-target-illuminator/carbine-target-illuminator-1.txt)
#### DESCRIPTION
Combined the timer and state/mode selector into a single MC6000, eliminating one MCxxxx chip.
#### PARTS
- 2x MC6000 HIGH PERFORMANCE MICROCONTROLLER
- 1x DX300 DIGITAL I/O EXPANDER
#### PERFORMANCE
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-1-stats.png)
#### DIAGRAM
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-1.png)

## [SOLUTION 3](/solutions/carbine-target-illuminator/carbine-target-illuminator-2.txt)
#### DESCRIPTION
Changed the states from [0, 1, 2] to [001, 010, 100], allowing me to send the state directly into the DX300, replacing one MC6000 with a MC4000.
#### PARTS
- 1x MC4000 HIGH PERFORMANCE MICROCONTROLLER
- 1x MC6000 HIGH PERFORMANCE MICROCONTROLLER
- 1x DX300 DIGITAL I/O EXPANDER
#### PERFORMANCE
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-2-stats.png)
#### DIAGRAM
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-2.png)

## [SOLUTION 4](/solutions/carbine-target-illuminator/carbine-target-illuminator-3.txt)
#### DESCRIPTION
Moved the state/mode selection into a table stored on an 200P-14 Read Only Memory Module.
#### PARTS
- 1x MC4000 HIGH PERFORMANCE MICROCONTROLLER
- 1x MC6000 HIGH PERFORMANCE MICROCONTROLLER
- 1x DX300 DIGITAL I/O EXPANDER
- 1x 200P-14 READ-ONLY MEMORY
#### PERFORMANCE
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-3-stats.png)
#### DIAGRAM
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-3.png)

## [SOLUTION 5](/solutions/carbine-target-illuminator/carbine-target-illuminator-4.txt)
#### DESCRIPTION
Added a second DX300 and and inverter, allowing me to do a tcp trick, further reducing the code and replacing the MC6000 with a MC4000X. 
#### Parts
- 1x MC4000X HIGH PERFORMANCE MICROCONTROLLER
- 1x MC6000 HIGH PERFORMANCE MICROCONTROLLER
- 1x DX300 DIGITAL I/O EXPANDER
- 1x 200P-14 READ-ONLY MEMORY
- 1x LC70G04 INVERTER
#### PERFORMANCE
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-4-stats.png)
#### DIAGRAM
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-4.png)

## SUPPLEMENTAL DOCUMENTATION
![](/solutions/carbine-target-illuminator/carbine-target-illuminator-supplemental.png)
