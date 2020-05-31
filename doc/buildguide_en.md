# Lily58 Build Guide


## Required parts

| Part Name | Quantity | Remarks |
| -------- | ------- | ------- |
| Lily58 PCB | 2 sheets ||
| Lily58 case | 1 set ||
| ProMicro | 2 pieces | Recommended to use [Consult] (https://yushakobo.jp/shop/a01mc-00/) as it can be replaced because it reduces the number of times of soldering and the connector is easily damaged. |
| Key switch (Cherry MX, PG1350) | 58pcs * | ALPS axis not supported |
| Keycap | 1U 56 pcs 1.5U 2 pcs * | 1.5U part can be 1U |
| Diode 1N4148 | 58 pieces ||
| Tact switch | 2 |
| TRRS Jack | 2 ||
| M2 spacer 6mm, 10mm | 10 pieces, 4 pieces ||
| M2 screw 5mm | 28 pieces ||
| TRS (TRRS) cable | 1 pc | Audio cable called AUX cable |
| Micro USB cable | 1 pc | Magnetic type is recommended due to low durability of the Pro Micro connector |

* Preparation is required as it is not included in the kit.


## Install the diode
** When using a low profile switch The surface mount diode (1N4148W) sold separately (http://akizukidenshi.com/catalog/g/gI-07084) is recommended.
When using the diode with a foot attached, it is necessary to minimize the protrusion of the soldered surface. (Cut the legs before soldering) **

This PCB is reversible, so we will mount the components on each side. The side on which the diode is mounted (the side where you can see the orange parts) is the back side.
![img_2008](https://user-images.githubusercontent.com/6285554/52172886-61d20700-27bc-11e9-888f-42a95c7dd569.JPG)
Seen from the side, it looks like this
! [PCB2](https://user-images.githubusercontent.com/6285554/51115630-2642bd80-184c-11e9-93e5-8f85ee5e45b0.png)

Bend the legs of the diode.
The legs of the diode can be easily bent by pressing the case with three stacked cases.
! [img_2009](https://user-images.githubusercontent.com/6285554/52172887-6ac2d880-27bc-11e9-9b3e-378a83c5a881.JPG)
 
 Insert the bent diode on the back side of the PCB (the side opposite the side where the switch or ProMicro is mounted).
The diode has an orientation. Check the notation on the PCB and insert it in the correct direction.
Solder with the black line of the diode always facing in the direction of the triangular bar on the board as shown in the image below. If the orientation is incorrect, the key will not respond.
! [46900579-542c0500-cedf-11e8-87a7-07f710f7e78e](https://user-images.githubusercontent.com/6285554/52002682-f7903c80-2505-11e9-907a-8407568322da.jpg)
! [diode](https://user-images.githubusercontent.com/6285554/48820707-83187f00-ed99-11e8-802e-90b23ca594a0.png)

Soldering is done from the back side, but it will fall off, so stop it with masking tape. To prevent the diode from floating when stopping, temporarily fix it while applying pressure from the top of the tape and holding it down.
! [img_2010](https://user-images.githubusercontent.com/6285554/52172891-829a5c80-27bc-11e9-81ab-878caa8645f6.jpg)
Solder.
! [unadjustednonraw_thumb_2d42](https://user-images.githubusercontent.com/6285554/52172899-b07fa100-27bc-11e9-9210-38bbdfb7d979.jpg)

After soldering, cut the diode legs with nippers. When you cut, your feet will fly easily, so be sure to hold your feet while cutting.
After cutting, attach 10mm (long spacer).
! [unadjustednonraw_thumb_2d48](https://user-images.githubusercontent.com/6285554/52172901-b07fa100-27bc-11e9-88a8-61a0eacfc6a4.jpg)

## Solder the TRRS jack / reset switch
Install the TRRS jack on the top left of the surface. Both of them are easy to drop or slip when turning over and soldering, so temporarily fix them with masking tape.
! [unadjustednonraw_thumb_2d4a](https://user-images.githubusercontent.com/6285554/52172948-8da1bc80-27bd-11e9-928b-fba7b8fa2b49.jpg)
Solder from the back side.
! [unadjustednonraw_thumb_2d4b](https://user-images.githubusercontent.com/6285554/52172964-e6715500-27bd-11e9-9b0a-4186301a1d56.jpg)


## When using for OLED (optional)
When using OLED, jumper the four pads near the ProMicro on the surface.
! [unadjustednonraw_thumb_2d41](https://user-images.githubusercontent.com/6285554/52172989-41a34780-27be-11e9-858a-cc69c2626160.jpg)

## Soldering the Pro Micro
   
#### When using Consru
If you use [Consult](https://yushakobo.jp/shop/a01mc-00/), please install it as follows.
Solder by referring to the ProMicro chapter of Helix's [Build Guide](https://github.com/MakotoKurauchi/helix/blob/master/Doc/buildguide_jp.md#pro-micro).
Solder only the ProMicro side, not the PCB side.
After soldering, insert it firmly so that it does not float.

### When using the attached pin
Take the Pro Micro out of its bag and insert it into the PCB with the long leg down and the row inside the red line in the image below marked by the ** PCB line. Please note that the insertion location is different on the left and right.

! [ProMicro_PCB](https://user-images.githubusercontent.com/6285554/48819671-6a599a80-ed94-11e8-8e5d-6a6abca326a7.png)

Mount the Pro Micro from above with the part-side down.
Solder the ProMicro side.
! [46900581-54c49b80-cedf-11e8-88e1-25a1a2fb378d](https://user-images.githubusercontent.com/6285554/52002684-f95a0000-2505-11e9-83f6-6eb3dc8f2a02.jpg)
! [46900582-54c49b80-cedf-11e8-9107-83038838a7da](https://user-images.githubusercontent.com/6285554/52002687-f9f29680-2505-11e9-9ecf-b7bf3ad9f270.jpg)

After soldering the ProMicro side, fix it with masking tape and solder from the back side of the board.
After soldering, use a nipper to cut off the extra pins.

## Attach the key switch
Fit the spacer and key switch in 4 places on the top plate, attach it to the PCB while being careful not to bend the pins, and check that there is no floating or tilting and solder the 4 switches.
! [unadjustednonraw_thumb_2d3e](https://user-images.githubusercontent.com/6285554/52173011-9a72e000-27be-11e9-9716-4c9a301c35ac.jpg)
! [4dabqoswsoi9o8wor3cdfg_thumb_2d49](https://user-images.githubusercontent.com/6285554/52173013-9fd02a80-27be-11e9-958e-54bb7e929f1d.jpg)

Attach the remaining switches to the top plate.
If it is installed properly, the legs of the pin will come out a little from the PCB, but if it is bent or not firmly attached, the legs will not come out as in the image below. If your leg is bent or it is not firmly attached to the plate, please remove it once and check.
Install and solder all switches.
! [48868154-037fc400-ee1c-11e8-9d45-b888f744387a](https://user-images.githubusercontent.com/6285554/52002691-fb23c380-2505-11e9-8fa1-c75d20d3636d.jpg)
! [switch](https://user-images.githubusercontent.com/6285554/48868657-b7ce1a00-ee1d-11e8-9346-9bfc967e95cf.png)

## Attach the ProMicro cover
Install the acrylic for the top of the Pro Micro.
Install with the wider side on the outside. Screw the top with a low head screw.
! [promicro_cover](https://user-images.githubusercontent.com/6285554/48837829-c4288780-edc9-11e8-8efb-6714d8e68e92.png)
! [unadjustednonraw_thumb_2d47](https://user-images.githubusercontent.com/6285554/52173081-ea9e7200-27bf-11e9-9551-3eb41a0389cb.jpg)
## Write keymap
Preparation is required to write the keymap. It is described on the assumption that it has been installed. [Please refer to the official qmk page etc. for reference. ](https://docs.qmk.fm/#/getting_started_build_tools)
  
If you use QMK Toolbox, you don't need to build environment and you can write in GUI. (Keymap cannot be changed)
[qmk / qmk_toolbox](https://github.com/qmk/qmk_toolbox/releases)

To write Lily58's default keymap run the following in the qmk_firmware folder hierarchy

    make lily58: default: avrdude


When ** Detecting USB port, reset your controller now ... ** is displayed, press the reset button on the keyboard to start writing.
Do the same for the other keyboard as above.

The default keymap is as follows.
! [lily58_default](https://user-images.githubusercontent.com/6285554/47273241-38ee8300-d5cc-11e8-9099-10c1b35e24fc.png)

## Operation check
Please connect the left and right with TRRS cable (TRS cable), connect the MicroUSB cable to ProMicro on the left side (in the case of default key map) and check if the key responds.
It is completed by attaching 4 rubber feet on the back side. Thank you for your hard work.
! [vu6sptlhszykivrvgkltyw_thumb_2d44](https://user-images.githubusercontent.com/6285554/52173150-795fbe80-27c1-11e9-8376-edc698e943e8.jpg)

! [47264498-53384a80-d553-11e8-907a-a03c6f2c5893](https://user-images.githubusercontent.com/6285554/52002699-fd861d80-2505-11e9-96a8-f58a93534255.jpg)

## In case of trouble
### Q. One-row (multi-row) or one-row (multi-row) key switch does not respond
A.ProMicro soldering and mounting may not be done properly. Please check again and re-solder if necessary.

### Q. The key switch does not respond by itself
A. There may be a problem with the key switch soldering or the diode soldering.

For key switch
Check the soldering of the defective key switch. If there is not enough solder, re-solder.
  
For diode soldering
Check the direction of the diode. If it is wrong, remove it and re-solder.
If the soldering is insufficient, re-solder it.

** If you have any problems, please feel free to send a message to the "# Lily58" channel of Discord server ([Self-Made Keyboards in Japan](https://discordapp.com/invite/NM7XtDW)) or Twitter: @F_YUUCHI **
