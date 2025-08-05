This quick-start guide will get you up and running with designing and building your own MOSAIC satellite. 

You should only follow this guide if you have all the necessary pieces of MOSAIC. If you don't have all the pieces of MOSAIC, then please see about acquiring what you need in the ["Getting Your Own MOSAIC" guide](https://www.mosaicsat.org/getting_mosaic/).

??? question "What are all the necessary MOSAIC pieces?"
    
    Use the following list to ensure you have everything needed to proceed with this quick-start guide. 

    - 1x Assembled MOSAIC Main Board
    - 1x Assembled MOSAIC Power Board
    - 1x Assembled MOSAIC ProtoBoard
    - All Pieces of MOSAIC's frame
    - 1x Choice of processor module
    - Choice of MOSAIC memory module(s)
    - Choice of sensors
    - All non-optional items listed in the [MOSAIC BOM](https://docs.google.com/spreadsheets/d/1xMUYyzwjdTFx7HzwNHd50U6s08wMuClfGDR2PERgSA4/edit?usp=sharing)

---

## Quick-Start Guide

<div class="grid cards" markdown>

-   :fontawesome-solid-screwdriver-wrench:{ .lg .middle } __Tools Needed__

    ---

    - Phillips head screwdriver for M2.5 and M3 screws

-   :fontawesome-solid-stopwatch:{ .lg .middle } __Time to complete__

    ---

    ~ 45 min.

-   :fontawesome-solid-gauge:{ .lg .middle } __Difficulty__

    ---

    Easy

</div>

The following are steps for quickly setting up your satellite:

---

## I. Choose your satellite's components

MOSAIC is customizable with several options to create a satellite tailored to your needs. The first step is to pick the modules you want for your satellite.

!!! info "Here's what you'll need to pick for your satellite:"

    - [x] 1x Processor for Main Board
    - [x] 1x transceiver
    - [x] Any number of Qwiic/STEMMA QT sensors or function board sensors
    - [x] Any number of MOSAIC memory modules

??? tip "Example setups coming soon"

    Example setups with pre-chosen components will be included on this site soon! These example setups will act as a good starting point for anyone making their own custom MOSAIC satellite.

### :octicons-arrow-right-24: :fontawesome-solid-microchip: Pick your processor

You will need a processor module to get started. MOSAIC is compatible with any of the MicroMod processors offered by Sparkfun Electronics. 

You can view the complete list of processor modules compatible with MOSAIC, including brief descriptions of each one and links to purchase them, [here](https://www.mosaicsat.org/core_documentation/hardware/main_board/processors/). 

### :octicons-arrow-right-24: :fontawesome-solid-tower-broadcast: Pick your transciever

Unfortunately, Sparkfun has discontinued the [recommended transceiver for MOSAIC](https://www.sparkfun.com/sparkfun-micromod-lora-function-board.html). Custom transceivers are currently being developed for the MOSAIC project. You will find them listed [here](https://www.mosaicsat.org/core_documentation/hardware/sensors_and_radios) when they're complete. 

### :octicons-arrow-right-24: :fontawesome-solid-flask: Pick your sensor(s)

You have two inclusive options for adding sensors to your satellite:

1. Include any [MicroMod-compatible function board](https://www.mosaicsat.org/core_documentation/hardware/main_board/function_boards/) to MOSAIC's Main Board. (Limit = 2 for MOSAIC Main Board)
2. Include any [Qwiic-compatible](https://www.sparkfun.com/sensors.html?sf_global_qwiic_connector=8262) or [STEMMA QT-compatible](https://www.adafruit.com/category/1005) sensors. These will be added to MOSAIC's ProtoBoard (see the hardware assembly section below).

Pick any number of these sensors to include with your satellite. The only restrictions are internal volume available, open ports, and power consumption limits.

### :octicons-arrow-right-24: :fontawesome-solid-sd-card: Pick your memory module(s)

There are two slots on MOSAIC's Main Board for adding expandable memory. It's recommended that you add at least one memory module for storing your sensor's data. 

You can find out more about MOSAIC's memory modules [here](https://www.mosaicsat.org/core_documentation/hardware/main_board/memory_modules/).

---

## II. Hardware Assembly

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

### :octicons-arrow-right-24: Attach brackets to MOSAIC boards

Each of MOSAIC's core PCBs (Main Board, Power Board, and ProtoBoard) requires two brackets to be attached to it. (Figure 12) These brackets will secure the boards to MOSAIC's frame. 

To attach these brackets:

1. Starting with any of MOSAIC's core boards, place a bracket on either side of the board at the flat edge of the board's outline so that the holes of the bracket line up with the holes of the board. 

    The flat edge of the bracket should be flush with the flat edge of the board. (Figure 13)

    !!! info "Brackets have two different pairs of holes"

        If you notice the bracket's holes don't align with the holes on the board, try flipping the bracket to the other side. The brackets have two pairs of holes for mounting to MOSAIC's boards and frame, respectively. These pairs of holes have different spacing.  

2. Secure the bracket to the board using the plastic screws and nuts from [MOSAIC's BOM](https://docs.google.com/spreadsheets/d/1xMUYyzwjdTFx7HzwNHd50U6s08wMuClfGDR2PERgSA4/edit?usp=sharing). (Figure 14)  

3. Place another bracket on the same side of the board but opposite edge and secure it to the board with plastic screws and nuts. (Figure 15)

4. Repeat steps 1 - 3 above for the two other MOSAIC core boards. 

??? tip "Tip: Start securing boards to frame"

    Before continuing with your satellite assembly and connecting everything, it may help to secure MOSAIC's three core boards to one of the x-y face pieces of MOSAIC's frame (see the image below). 

    This is based on preference. Some may secure the boards to the frame piece now to determine how everything will fit together, while others prefer to keep their boards off the frame until the end for easy access. 

### :octicons-arrow-right-24: Adhere solar cells to frame pieces

Each face of MOSAIC's frame can hold up to two solar cells. 

These cells adhere to the frame using double-sided tape (or any other adhesive you prefer), and the cables of the cells are wired into the interior of the satellite through openings in the frame pieces. (Figure 16)

You can choose any orientation or placement of these cells on the frame that meets your needs. You may even omit any number of them from your satellite. 

You need to be mindful not to cover anything important. For example, the USB port on the Main Board of your satellite will be accessed from outside the frame. You want to ensure that no solar cells cover the USB. (Figure 17)

To secure your solar cells to MOSAIC's frame pieces:

1. Orient a cell onto the faces of the frame where you would like it to be. 

    Ensure that you can still wire the cable from the cells to the other side of the face and that the cells do not cover anything important.

2. Note where the back of the cell makes contact with MOSAIC's frame.

3. Move the cell and place double-sided tape (or other adhesive) onto the frame where the cell made contact. (Figure 18)

4. Return the cell to its original position, feeding its cable to the other side of the face, then press the cell against the adhesive.

5. Repeat steps 1 - 4 above for all other cells you wish to include. 

