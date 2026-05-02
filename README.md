# Thrustmaster FGT translator

This is a little microcontroller used to adjust pedals for the Thrustmaster Ferrari GT/Challenge wheel.

![render of the pcb](/readme-assets/pcb.png)

![render of it assembled with the case](/readme-assets/assembled-case.png)

## Parts

- STM32G071GBU6
- 1x 0402 100nF cap
- 1x 0402 4.7uF cap
- 1x TS-1088-AR02016 (switch)
- 2x 1x3 P2.54mm pinheaders
- 2x 1x4 P2.54mm pinheaders

## Microcontroller 3D model

In accordance with the terms of SnapMagic's terrible license, I can't redistribute the microcontroller 3D model, hence it's not included. If you want it, it's on Digikey.

## CAD

All STEP files are provided in `./CAD/`. Design was done in Onshape, but assembly was done in FreeCAD. The assembly design file is in CAD, while here are the Onshape design files:

- [case top](https://cad.onshape.com/documents/4cd0723182fb444a0eb40fc6/w/16d03d3cdb549aa466cdaea8/e/f06282226fc81b6d0f6ad971)
- [case bottom](https://cad.onshape.com/documents/cf5c5eb7a78b451ade18eba2/w/7ba96a54e81cf9eb85f76eec/e/e2db873006224d9eaa981bd6)

I can't really test if just providing the links works so uh. Good luck, let me know if you can't access them.

## Wiring

Reference the schematic for wiring on the PCB side, this is the pinout of the cable.

![](/readme-assets/pinout.png)
