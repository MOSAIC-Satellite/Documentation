This page will guide you through 3D printing the frame for your MOSAIC satellite, whether you have a 3D printer or need to order prints online. You'll find links to the necessary files, a breakdown of the frame's structure, assembly tips, and suggestions for printing services if you don't own a 3D printer.

<div class="grid cards" markdown>

-   :fontawesome-solid-screwdriver-wrench:{ .lg .middle } __Tools Needed__

    ---

    - Computer 
    - Super glue
    - (Optional) 3D printer
    - (Optional) Filament for 3D printer

-   :fontawesome-solid-stopwatch:{ .lg .middle } __Time to complete__

    ---

    ~ 12 hours (if printing yourself)

-   :fontawesome-solid-money-bills:{ .lg .middle } __Estimated Cost__

    ---

    Varies depending on whether you are printing yourself or having your prints made.

-   :fontawesome-solid-gauge:{ .lg .middle } __Difficulty__

    ---

    Moderate

</div>

---

## About the MOSAIC 3D Printed Frame

The MOSAIC satellite's frame is fully 3D printable and modular, designed for rapid assembly and easy modification (Figure 1). The frame consists of:

- 2x x-y face pieces

- 2x Removable top/bottom (z face) panels (attached to the x-y face pieces using screws)

- Interior 3D printed brackets for securely mounting MOSAIC's core circuit boards

Follow the steps below to fabricate your MOSAIC frame.

---

## I. Downloading the 3D models

All necessary .stl files are provided via the MOSAIC GitHub repository

1. Visit the [MOSAIC frame GitHub repository](https://github.com/MOSAIC-Satellite/frame/tree/main).
2. Click on the green `<> Code` button next to the "About" section of the repository, then click `Download ZIP` (Figure 2). This will download the entire repository in a ZIP folder.
3. Unzip (extract) the folder to any location on your computer. 

You’ll need three .stl files to print a complete frame set:

- X-Y Face Piece (`mosaic_xyface.stl`)
- Z Face Panels (`mosaic_zface.stl`)
- Bracket (`mosaic_bracket.stl`)

These files are all found in the `Model_Files` folder of the repository you downloaded.

---

## II. Print Your MOSAIC frame pieces

Using your 3D printer, print all the pieces of MOSAIC's frame from the .stl files downloaded in the previous step. The following quantities are what you need to print of each .stl file to have a complete MOSAIC frame:

- 2x `mosaic_xyface.stl`
- 2x `mosaic_zface.stl`
- 6x `mosaic_bracket.stl` (two for each of MOSAIC's core circuit boards)

??? info "Printing Tips"
    - **Material**: PLA is recommended for educational use and ease of printing, but PETG or ABS can provide additional strength if required.
    - **Layer Height**: 0.2 mm gives good resolution without excessive print times.
    - **Infill**: 20–30% is typically sufficient for structural parts.
    - **Supports**: The frame pieces are designed to minimize support needs, but check orientation before slicing.

---

## III. (Optional) Glue plastic nuts into frame pieces

The two x-y face pieces and the brackets all have slots that fit the plastic nuts purchased from MOSAIC's BOM. (Figure 3) The plastic nuts act as threading for the plastic screws that secure the frame pieces together. 

It's recommended that you glue the nuts into their slots. This makes the final assembly of your satellite easier. 

1. Apply a small amount of glue to the inner edges of each of the two nut slots on one of the x-y face pieces. (Figure 4)

    !!! tip

        You don't want to apply too much glue. Otherwise, you will end up with a mess and/or a clogged nut. It may be helpful to use a suitable applicator for the glue, such as a Q-Tip. The glue listed in [MOSAIC's BOM](https://docs.google.com/spreadsheets/d/1xMUYyzwjdTFx7HzwNHd50U6s08wMuClfGDR2PERgSA4/edit?usp=sharing) comes with a brush to facilitate application. 

2. Insert a plastic nut into each of these slots and allow to dry. (Figure 5)

3. Repeat steps 1 - 2 above for the two slots on the other x-y face piece and the four slots on each of the brackets. 

---

## Getting your frame printed without a 3D printer

If you don’t have access to a 3D printer, you may look into the following options instead:

- **Online 3D Printing Services**: Upload the downloaded .stl files to services like

    - [Shapeways](https://www.shapeways.com/)

    - [Treatstock](https://www.treatstock.com/)

    - [3D Hubs](https://www.hubs.com/) (now known as Protolabs Network)

- **Local Makerspaces and Libraries**: Many community makerspaces and public libraries offer 3D printing for a nominal fee. Search for “makerspace” or “3D printing” plus your city name.

- **University Labs**: If you are affiliated with an educational institution, check if their engineering or fabrication labs can help.

??? note "How to order"
    
    - Download the .stl files from GitHub (step I above).

    - Upload/bring them to the service of your choice.

    - Specify material and print settings if possible.

    - Order at least two main frame pieces, two z-face panels, and as many brackets as needed.

---

[:octicons-arrow-left-24: Back to step 3](https://www.mosaicsat.org/getting_mosaic/self_assemble/assemble_boards/){ .md-button } [Next to What's Next? :octicons-arrow-right-24:](https://www.mosaicsat.org/getting_mosaic/self_assemble/whats_next/){ .md-button }