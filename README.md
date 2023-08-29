# megacell_mospatch

This is a hardware patch for the megacell charger that uses TP4056 charging IC's.
The purpose of this patch is to fully open the mosfets for reverse polarity protection,
improving the voltage reading while charging or discharging a cell. The RDS-ON of the mosfet
being highly lowered and being constant so it can be offset for in software.


The connection mode:

1. Placed on the bottom side of the PCB facing up.
2. Remove the resistor from the gate of the mosfet (pictures coming soon)
3. Connect the 5V +, GND and 3.3V wires to the PCB
4. Connect C+ from each cell to coresponding ports on the PCB
5. Connect the corespoding C#_Gate to the gate of the reverse polarity mosfet.

The mod is complete, check the voltage of the gate when voltage of the cell goes above 0.7 volts.
The gate voltage should be around 5V when it's on.


The files are made for JLCP PCB website to order already assembled PCB.