<div class="grid cards" markdown>

-   :fontawesome-solid-screwdriver-wrench:{ .lg .middle } __Tools Needed__

    ---

    - Computer

-   :fontawesome-solid-stopwatch:{ .lg .middle } __Time to complete__

    ---

    ~ 10 min.

-   :fontawesome-solid-gauge:{ .lg .middle } __Difficulty__

    ---

    Easy

</div>

---

MOSAIC is customizable with several options to create a satellite tailored to your needs. The first step is to pick the modules you want for your satellite.

!!! info "Here's what you'll need to pick for your satellite:"

    - [x] 1x Processor for Main Board
    - [x] 1x transceiver
    - [x] Any number of Qwiic/STEMMA QT sensors or function board sensors
    - [x] Up to 2 MOSAIC memory modules

??? tip "Example setups coming soon"

    Example setups with pre-chosen components will be included on this site soon! These example setups will act as a good starting point for anyone making their own custom MOSAIC satellite.

### :octicons-arrow-right-24: :fontawesome-solid-microchip: Pick your processor

You will need a processor module to get started. MOSAIC is compatible with any of the MicroMod processors offered by Sparkfun Electronics. 

You can view the complete list of processor modules compatible with MOSAIC, including brief descriptions of each one and links to purchase them, [here](https://www.mosaicsat.org/core_documentation/hardware/main_board/processors/). 

If you're new to microprocessors, the [ESP32](https://www.sparkfun.com/sparkfun-micromod-esp32-processor.html) or [RP2040](https://www.sparkfun.com/sparkfun-micromod-rp2040-processor.html) are good options for beginners as they have well-detailed documentation.

### :octicons-arrow-right-24: :fontawesome-solid-tower-broadcast: Pick your transciever

Unfortunately, Sparkfun has discontinued the [recommended transceiver for MOSAIC](https://www.sparkfun.com/sparkfun-micromod-lora-function-board.html). Custom transceivers are currently being developed for the MOSAIC project. You will find them listed [here](https://www.mosaicsat.org/core_documentation/hardware/sensors_and_radios) when they're complete. 

In the meantime, consider choosing the [nRF52840](https://www.sparkfun.com/sparkfun-micromod-nrf52840-processor.html) or [ESP32](https://www.sparkfun.com/sparkfun-micromod-esp32-processor.html) microprocessors for your satellite. Both have built-in Bluetooth capabilities that can allow you to transmit and receive data wirelessly from your satellite. 

### :octicons-arrow-right-24: :fontawesome-solid-flask: Pick your sensor(s)

You have two inclusive options for adding sensors to your satellite:

1. Include any [MicroMod-compatible function board](https://www.mosaicsat.org/core_documentation/hardware/main_board/function_boards/) to MOSAIC's Main Board. (Limit = 2 for MOSAIC Main Board)
2. Include any [Qwiic-compatible](https://www.sparkfun.com/sensors.html?sf_global_qwiic_connector=8262) or [STEMMA QT-compatible](https://www.adafruit.com/category/1005) sensors. These will be added to MOSAIC's ProtoBoard in the hookup guide.

Pick any number of these sensors to include with your satellite. The only restrictions are internal volume available, open ports, and power consumption limits.

### :octicons-arrow-right-24: :fontawesome-solid-sd-card: Pick your memory module(s)

There are two slots on MOSAIC's Main Board for adding expandable memory. It's recommended that you add at least one memory module for storing your sensor's data. 

You can find out more about MOSAIC's memory modules [here](https://www.mosaicsat.org/core_documentation/hardware/main_board/memory_modules/).