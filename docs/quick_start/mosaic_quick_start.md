This quick-start guide will get you up and running with designing and building your own MOSAIC satellite. 

You should only follow this guide if you have all the necessary pieces of MOSAIC. If you don't have all the pieces of MOSAIC, then please see about acquiring what you need in the ["Getting Your Own MOSAIC" guide](https://www.mosaicsat.org/getting_mosaic/).

??? question "What are all the necessary MOSAIC pieces?"
    
    Use the following list to ensure you have everything needed to proceed with this quick-start guide. 

    - 1x Assembled MOSAIC Main Board
    - 1x Assembled MOSAIC Power Board
    - 1x Assembled MOSAIC ProtoBoard
    - All Pieces of MOSAIC's frame
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

- Connect the sensors using a Qwiic cable inserted into any of the Qwiic ports on the ProtoBoard (Figure 10) or connect the soldered-on header pins to the appropriate I^2^C through-hole pin. (Figure 11) Be sure to leave one of the Qwiic ports on the ProtoBoard free. This port will connect your sensors to MOSAIC's Main Board (done in a future step).

### :octicons-arrow-right-24: Attach brackets to MOSAIC boards

