# Main Pinout

The design this year has one gigantic pinout that connects the Connector, Auxiliary, and Power boards.

The pinout can be found on the Google Drive via [here](https://docs.google.com/spreadsheets/d/12fttB78_SGGhG3ety12AxKMyCXqxlnrm3WpfixTQAak/edit?usp=sharing).
*Note: one must use their OSU email to access the document* 

## Motivation

The current pinout was designed with two specifications in mind: that there would be an even distribution of ground pins for the power pins and analog signal paths, and that it would be possible to connect the [Orbitty Carrier](https://connecttech.com/ftp/pdf/CTIM-ASG003_Manual.pdf) to our custom boards with a 20-pin ribbon cable.  The Orbitty Carrier simplifies interfacing with the ROV's main processor---the NVIDIA Jetson TX1.

## Pictures

### Schematic

Here is what the pinout looks like in the schematic on CircuitMaker.

<img src="https://ik.imagekit.io/kjbx6tb5231/2020-2021/pinout-main_MxXAT4fKG.png" alt="pinout schematic" style="width:80%;height:100%">

### 2D

Here is what part of the pinout (the P1 connector in this case) looks like on a PCB in 2d view.  Notice that the implementation on the board has a different orientation than that of the schematic. This is just how the header got put onto the board.  The important part is that, looking with the receiving part of the header facing the viewer, the 5V_OUT pin is on the top right corner.  This orientation allows for a 20-pin connector to attach the custom boards to the Orbitty.

<img src="https://ik.imagekit.io/kjbx6tb5231/2020-2021/pinout-2d_z3rd6G2a7s.png" alt="pinout section PCB: 2d" style="width:80%;height:100%">

### 3D

Here is the 3d view of the connector on the PCB looking at the same section as above.

<img src="https://ik.imagekit.io/kjbx6tb5231/2020-2021/pinout-3d_2dr1uYV8p.png" alt="pinout section PBC: 3d" style="width:80%;height:100%">

