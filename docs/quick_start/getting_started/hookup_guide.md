<div class="grid cards" markdown>

-   :fontawesome-solid-screwdriver-wrench:{ .lg .middle } __Tools Needed__

    ---

    - Phillips head screwdriver for M2.5 and M3 screws

-   :fontawesome-solid-stopwatch:{ .lg .middle } __Time to complete__

    ---

    ~ 15 min.

-   :fontawesome-solid-gauge:{ .lg .middle } __Difficulty__

    ---

    Easy

</div>

---

### :octicons-arrow-right-24: Connect your processor, memory module(s), and RBF pin

1. Your processor board connects to MOSAIC's Main board using the M.2 form factor. 

    Insert the key of your processor board (Figure 1) into the M.2 slot on the Main Board labeled "Processor" at an angle of about 25°. (Figure 2)

- Once the board is in the socket, gently push and hold the processor board down and tighten the screw with a Phillips head. (Figure 3)

- Connect your memory module to one of the slots labeled "Memory" and secure it to the board using the same process as the processor board above.

- Insert the remove before flight (RBF) pin (the 3.5 mm audio plug keychain) into the 3.5 mm audio jack on the top of the Main Board. (Figure 4)

### :octicons-arrow-right-24: Connect your function board(s)

If you're using any MicroMod-compatible [function boards](https://www.mosaicsat.org/core_documentation/hardware/main_board/function_boards/), insert them into the M.2 slots labeled "Function board" on the back of MOSAIC's Main Board. The process of adding these boards is similar to adding a processor above. 

1. Insert the key of your processor board into the M.2 slot on the Main Board labeled "Processor" at an angle of about 25°. If adding two function boards, insert them both now. (Figure 5)

- Gently hold down the function board(s) and tighten the screw between the two function board slots with a Phillips head. (Figure 6)

- Tighten the screw(s) on the other side(s) of the function board(s) with a Phillips head. (Figure 7)

### :octicons-arrow-right-24: Connect sensors to MOSAIC's ProtoBoard

MOSAIC's [ProtoBoard](https://www.mosaicsat.org/core_documentation/hardware/protoboard/) serves as a carrier for the satellite's sensors. You can mount Qwiic/STEMMA QT compatible sensors to the board using the various mounting holes or solder the sensor directly to the board. 

Sensor data is sent to the satellite's processor using the I^2^C protocol through [Qwiic connectors](https://www.sparkfun.com/qwiic). 

1. Mount any number of your sensors to MOSAIC's ProtoBoard using M2.5 standoffs in the mounting holes (Figure 8) or solder them to the ProtoBoard using header pins. (Figure 9)

- Connect the sensors using a Qwiic cable inserted into any of the Qwiic ports on the ProtoBoard, (Figure 10) or connect the soldered-on header pins to the appropriate I^2^C through-hole pin. (Figure 11) Be sure to leave one of the Qwiic ports on the ProtoBoard free. This port will connect your sensors to MOSAIC's Main Board (done in a future step).