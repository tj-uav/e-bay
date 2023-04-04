# e-bay
Electronics bay PCB for avalon

See Avalon X -> Improvements -> Ebay for the full MCAD assembly.

Designed to take 3-4S battery input through an XT60 connector and power a Pixhawk 2.4.8, Raspberry Pi 4, 5.5V Servo rail, Bullet AC, camera gimbal, plus one extra XT60 connector. Requires three buck converter modules (The servo rail buck must be rated for 5A, the other two may be between 3A and 5A). The Raspberry Pi buck module should be set to 5V flat. The Pixhawk buck module should be set to around 5.3V. The servo rail buck module should be set to 5-5.5V. Use a wire to connect the two PCBs, with the left side PCB receiving power from the battery and the right side PCB receiving power from the left. Because of a CAD mistake, the wire needs to be soldered to the right side PCB, while the left side can support an XT60 connector. Use 16AWG or thicker wire to handle high ish currents.

Molex cables going to the Pixhawk should have the same pinout on both ends of the cable (i.e. pin 1 is power). This is opposite of pixhawk convention, which mirrors the connector pinout on either end. Do NOT use pixhawk cables on this PCB.
