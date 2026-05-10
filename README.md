# Thrustmaster FGT translator

This is a little microcontroller used to adjust pedals for the Thrustmaster Ferrari GT/Challenge wheel. It takes the potentiometer values, adjusts them to match that the controller expects, and outputs the values through the DACs to the rest of the controller.

![render of the pcb](/readme-assets/pcb.png)

![render of it assembled with the case](/readme-assets/assembled-case.png)

## Parts

- STM32G071GBU6
- 1x 0402 100nF cap
- 1x 0402 4.7uF cap
- 1x TS-1088-AR02016 (switch)
- 2x 1x3 P2.54mm pinheaders
- 2x 1x4 P2.54mm pinheaders

## BOM

|Item                        |URL                                              |Price |Quantity needed|Quantity to order|Total|
|----------------------------|-------------------------------------------------|------|---------------|-----------------|-----|
|STM32G071GBU6               |<https://www.lcsc.com/product-detail/C529347.html> |1.65  |1              |1                |1.65 |
|100nF cap                   |<https://www.lcsc.com/product-detail/C60474.html>  |0.0011|1              |100              |0.11 |
|4.7uF cap                   |<https://www.lcsc.com/product-detail/C23733.html>  |0.0059|1              |50               |0.295|
|TS-1088-AR02016 (pushbutton)|<https://www.lcsc.com/product-detail/C720477.html> |0.0558|1              |10               |0.558|
|PZ254V-11-04P               |<https://www.lcsc.com/product-detail/C2691448.html>|0.0254|2              |20               |0.508|
|PZ254V-11-03P               |<https://www.lcsc.com/product-detail/C2937625.html>|0.0186|2              |50               |0.93 |
|                            |                                                 |      |               |                 |     |
|                            |                                                 |      |               |                 |     |
|Subtotal                    |4.06                                             |      |               |                 |     |
|Shipping and handling       |11.72                                            |      |               |                 |     |
|PCB                         |5.22                                             |      |               |                 |     |
|                            |                                                 |      |               |                 |     |
|**Total**                       |22.7325                                          |      |               |                 |     |

## Microcontroller 3D model

In accordance with the terms of SnapMagic's terrible license, I can't redistribute the microcontroller 3D model, hence it's not included. If you want it, it's on Digikey.

## CAD

All STEP files are provided in `./CAD/`. Design was done in Onshape, but assembly was done in FreeCAD. The assembly design file is in CAD, while here are the Onshape design files:

- [case top](https://cad.onshape.com/documents/4cd0723182fb444a0eb40fc6/w/16d03d3cdb549aa466cdaea8/e/f06282226fc81b6d0f6ad971)
- [case bottom](https://cad.onshape.com/documents/cf5c5eb7a78b451ade18eba2/w/7ba96a54e81cf9eb85f76eec/e/e2db873006224d9eaa981bd6)

I can't really test if just providing the links works so uh. Good luck, let me know if you can't access them.

## Wiring

The wiring is a 1-to-1 copy of the original board - wire the 4-pin to the left connector (J1, italicized). But for reference, this is the pinout of the RJ9 (board connector is the same)

![](/readme-assets/pinout.png)

And the pinout of the PCB:

![](/readme-assets/pcb-pinout.png)
