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

- 2x x-y face panels

- 2x z face panels (attached to the x-y face pieces using screws)

- Interior 3D printed brackets for securely mounting MOSAIC's core circuit boards

<figure markdown="span">
![Figure 1](images\frame_pieces.png)
    <figcaption>**Figure 1**: MOSAIC's frame pieces</figcaption>
</figure>

Follow the steps below to fabricate your MOSAIC frame.

---

## I. Downloading the 3D models

All necessary .stl files are provided via the MOSAIC GitHub repository

1. Visit the [MOSAIC frame GitHub repository](https://github.com/MOSAIC-Satellite/frame/tree/main).
2. Click on the green `<> Code` button next to the "About" section of the repository, then click `Download ZIP` (Figure 2). This will download the entire repository in a ZIP folder.

    <figure markdown="span">
    ![Figure 2](images\frame_github.png)
      <figcaption>**Figure 2**: Location where to download the needed files for MOSAIC's frame in the frame repository</figcaption>
    </figure>

3. Unzip (extract) the folder to any location on your computer. 

You’ll need three .stl files to print a complete frame set:

- X-Y Face Panel (`mosaic_xyface.stl`)
- Z Face Panel (`mosaic_zface.stl`)
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

<figure markdown="span">
![Figure 3](images\nut_and_slot.jpg)
    <figcaption>**Figure 3**: Plastic nut and corresponding slot on MOSAIC bracket piece</figcaption>
</figure>

It's recommended that you glue the nuts into their slots. This makes the final assembly of your satellite easier. 

1. Apply a small amount of glue to the inner edges of each of the two nut slots on one of the x-y face pieces. (Figure 4)

    <figure markdown="span">
    ![Figure 4](images\adding_glue.jpg)
      <figcaption>**Figure 4**: Adding super glue to the plastic nut slot on one of MOSAIC's bracket pieces</figcaption>
    </figure>

    !!! tip

        You don't want to apply too much glue. Otherwise, you will end up with a mess and/or a clogged nut. It may be helpful to use a suitable applicator for the glue, such as a Q-Tip. The glue listed in [MOSAIC's BOM](https://docs.google.com/spreadsheets/d/1xMUYyzwjdTFx7HzwNHd50U6s08wMuClfGDR2PERgSA4/edit?usp=sharing) comes with a brush to facilitate application. 

2. Insert a plastic nut into each of these slots and allow to dry.

3. Repeat steps 1 - 2 above for the two slots on the other x-y face piece and the four slots on each of the brackets. 

---

## IV. Adhere solar cells to frame pieces

Each face of MOSAIC's frame can hold up to two solar cells. 

These cells adhere to the frame using double-sided tape (or any other adhesive you prefer), and the cables of the cells are wired into the interior of the satellite through openings in the frame pieces. (Figure 5)

<figure markdown="span">
![Figure 5](images\cell_position.png)
    <figcaption>**Figure 5**: Position of a solar cell on MOSAIC's xy-face frame piece (a) and its power cable fed into the interior of MOSAIC's frame (b)</figcaption>
</figure>

You can choose any orientation or placement of these cells on the frame that meets your needs. You may even omit any number of them from your satellite. 

You need to be mindful not to cover anything important. For example, the USB-C port on the Main Board of your satellite will be accessed from outside the frame. You want to ensure that no solar cells cover the USB-C port. (Figure 6)

<figure markdown="span">
![Figure 6](images\cell_cover_uncover.png)
    <figcaption>**Figure 6**: Solar cell position that covers MOSAIC's Main Board USB-C port (a) and positioned so that nothing is being covered up (b)</figcaption>
</figure>

To secure your solar cells to MOSAIC's frame pieces:

1. Orient a cell onto the faces of the frame where you would like it to be. 

    Ensure that you can still wire the cable from the cells to the other side of the face and that the cells do not cover anything important.

2. Note where the back of the cell makes contact with MOSAIC's frame.

3. Move the cell and place double-sided tape (or other adhesive) onto the frame where the cell made contact. (Figure 7)

    <figure markdown="span">
    ![Figure 7](images\adhesive_positioning.png)
    <figcaption>**Figure 7**: Find where you'd like to position your solar cell on MOSAIC's face (a), then add adhesive where the cell made contact with the face (b - red bars)</figcaption>
    </figure>

4. Return the cell to its original position, feeding its cable to the other side of the face, then press the cell against the adhesive.

5. Repeat steps 1 - 4 above for all other cells you wish to include. 

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