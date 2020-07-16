Nexys Video OLED Demo
==============
 
Description
--------------
This project is a Vivado demo using the Nexys Video's LEDs, pushbuttons and OLED Display written in Verilog. When programmed onto the board,  the display will automatically be initialized. When you are done operating the demo, and want to turn your board off, press the CPU Reset Button to turn the display off. LED0 is tied to the status of the OLED display. If the LED0 is on so is the OLED display. The display can be turned on from an off state by pressing the CPU Reset Button again. The OLED Display is controlled by the BTNU, BTNC and BTND of the D-Pad Buttons as shown in the table below.

| Button      | Function                                                           |
| ----------- | -----------------------------------------------------------------  |
| BTNC        | With the display on, each pixel on the display can                 | 
|             | be lit up at once by pressing the center D-Pad button (BTNC).      |
|             | Press the BTNC to return the display to its original state         |
| BTNU        | With the display on, you can load pre-defined text onto the        |
|             | display by pressing the up D-Pad button (BTNU)                     |                          
| CPU_RESET   | The OLED display can be turned on and off by pressing the CPU      |
|             | Reset Button (CPU_RESET)                                           |
| BTND        | To clear the display, press the down D-Pad button (BTND)           |

Important Warning
--------------
Make sure to turn off the OLED display before shutting down or reprogramming your board.
  
Requirements
--------------
* **Nexys Video**:To purchase a Nexys Video, see the [Digilent Store](https://store.digilentinc.com/nexys-video-artix-7-fpga-trainer-board-for-multimedia-applications/)
* **Vivado 2020.1 Installation**:To set up Vivado, see the [Installing Vivado and Digilent Board Files Tutorial](https://reference.digilentinc.com/vivado/installing-vivado/start).
* **MicroUSB Cable**
* **12 Volt Power Supply**
 
Demo Setup
--------------
1. Download and extract the most recent release ZIP archive from this repository's [Releases Page](https://github.com/Digilent/Nexys-Video-OLED/releases).
2. Open the project in Vivado 2020.1 by double clicking on the included XPR file found at "\<archive extracted location\>/vivado_proj/Nexys-Video-OLED.xpr".
3. In the Flow Navigator panel on the left side of the Vivado window, click **Open Hardware Manager**.
4. Plug the Nexys Video into the computer using a MicroUSB cable.
5. In the green bar at the top of the Vivado window, click **Open target**. Select **Auto connect** from the drop down menu.
6. In the green bar at the top of the Vivado window, click **Program device**.
7. In the Program Device Wizard, enter "\<archive extracted location\>vivado_proj/Nexys-Video-OLED.runs/impl_1/top.bit" into the "Bitstream file" field. Then click **Program**.
8. The demo will now be programmed onto the Nexys Video. See the Description section of this README to learn how to interact with this demo.

Next Steps
--------------
This demo can be used as a basis for other projects, either by adding sources included in the demo's release to those projects, or by modifying the sources in the release project.
 Check out the Nexys Video's [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/nexys-video/start) to find more documentation, demos, and tutorials.
 For technical support or questions, please post on the [Digilent Forum](https://forum.digilentinc.com).

Additional Notes
--------------
For more information on how this project is version controlled, refer to the [Digilent Vivado Scripts Repository](https://github.com/digilent/digilent-vivado-scripts)
