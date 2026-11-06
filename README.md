
# Modern TRS-80 Model 1 Keyboard

## Introduction

This is a modern take on a TRS-80 Model 1 Keyboard.
It provides and identical (mostly) layout familiar to most people, 
And is based on a modern mechanical keyboard design.

The main features are:

* Uses standard ANSI (US) keyboard layout.
* Follows the 65% (with 67 keys) keyboard design.
* Uses MX key switches and standard ANSI keycaps
* Utilises hot-swappable key switchs.
* Supports either PCB (Cherry) or Plate mounted stabilisers.
* Optional CTRL, CAPS, FN, F1, F2, F3 keys with suitable software

A modern mechanical keyboard is built in layers the following is a 
Explosion of a modern typical keyboard

<PIC>

## Keyboard Design

The keyboard layout is based on the 65% (67 key) keyboard layout. 
This is similar to a keyboard on a laptop without the function key row.
The keyboard design utilises 64 of these keys, 5 of which are optional.

Most keys have 1 to 1 replacements on the modern keyboard except for 
the Break, and Clear keys. I chose to use the ESC and Home keys as 
substitutes. You can get custom key caps, but this is not required

Also there are two duplicate keys Left and Right arrow keys are 
mapped to Delete, and Tab keys.

An upgraded Level 2 ROM provides support for the modified key mappings
e.g. several shifted number keys map to different symbols.

## Components Provided

What is provided as part of this project

* 3D Printed Internal mounting frame
* 3D Printed case top bezel
* Keyboard PCB with Hot-swappable key switches.
* Level 2 ROM supporting changed key mappings.

As well as the components needed to build the PCB (see BOM) you will also 
need (8x) M2 bolts to mount the PCB, and matching heat set inserts.

## Keyboard Components

In addition to the components provided in this project you also need 
to source the following keyboard components

* MX Keycaps, with style matching your needs.
* MX Key Switches, any brand and type (not low profile) will do.
* MX Key Stabilisers, either PCB or Plate mounted are supported.
* Keyboard Plate (67 key) compatible with the chosen stabilisers.
* Keyboard Poron foam layers for cushioning and noise isolation.

There are 2 options to purchase these components
* Source the components separately from one or more suppliers.
* Purchase a suitable donor keyboard that contains all the components. 

### Separate Purchase

If purchasing separately you need to find compatible (keyboard layout) components.
While the Keycaps and key switches are interchangeable between most keyboards
There are some small exceptions like key width e.g. spacebar is 6.25U (wide).

In terms of stabilisers there are 2 types PCB mounted (Cherry) and Plate mounted. In either case you need to get a Plate that supports these stabilisers, and suitable stabilisers.

I have uncovered several DIY keyboards that have the same basic layout, and
Could be used to source the custom plate and foam kits.
* Tofu65 v3
* Bakeneko65 v3
* Neo65
* Zen65
* Lucky65

### Donor Keyboard

For my build I choose the “Epomaker Alua F65 (Blue)” keyboard. At the time of writing it is listed as $65 USD (on official website), but can be found cheaper depending on where you buy it.

https://epomaker.com/products/epomaker-aula-f65

Of course any keyboard can be used, the most important thing is to look for a hot-swappable keyboard with the matching key arrangement. Pay careful attention to the bottom row, and right column).

The only slight disadvantage of this keyboard was it didn’t have a “Home” (to replace Clear) key so I choose to use the “Delete” key instead. 

## Build

### PCB

Refer to the BOM for the components required, the main items are the “Kailh Low Profile Hot-swappable Socket”, and 3x 74LS00 series logic chips.

Notes when assembling the PCB

* All the components (except the power LED) are soldered to the back of the PCB.
* The power LED is considered optional, it can be omitted if not required.
* If using PCB mounted stabilisers (not in BOM) these need to be attached to the PCB.
* You can use IC sockets (or not) based on your preference

I suggest using the FFC ribbon cable to attach the keyboard to the main board, 
but a standard 20 pint header can also be used. Neither of these is in the BOM

### Internal Frame

The (3D Printed) internal frame mounts to 5 keyboard case mount points, 
and additionally it is supported from underneath by 3 central mounting posts.

The internal frame cannot be printed on a typical size 3D Printer and 
has been broken into 2 pieces using a connecting dovetail joint.
The internal frame can be printed in any material (I used PLA), since the part
Is quite thick, and well supported in the case.
The dovetail is tapered, and can only be joined in one way.
Ideally CA glue or epoxy should be used when joining the 2 parts.

Brass M2 heat set inserts are installed into the frame for the PCB to attach to.

Surrounding the PCB area is a brim which the keyboard plate rests on.
This provides support to the keys via the plate, removing stress on the PCB.
While the plate rests on the brim, it should not extend over it, and may need to be trimmed.

### Main Assembly

Assembly of the keyboard is done in layers, starting with the 3D printed internal frame.

Order of assembly
* Heat set screw inserts (8x) need to be melted into the standoffs in the frame.
* Foam layer under keyboard, this might be stuck to PCB back
* The main keyboard PCB itself, ensure it is fully assembled first.
* Use short M2 screws to attach the PCB to the internal frame.
* Thin cotton/plastic isolation layers, that sit under (and isolate PCB) the switches.
* Thick main sound deadening Poron Isolation Foam.
* The keyboard plate, including plate mounted key stabilisers.
* Key switches installed through plate into sockets, secures the plate
* Keycaps.

When installing each layer you need to ensure that foam layers are
trimmed fit within the outline of the PCB, so the sit down inside the brim of the internal frame;
and holes are added to allow PCB mounting screws to be used.

The keyboard plate may need to be trimmed, so it sits on the brim but doesn’t extend over it.
A cutout in the plate will also need to be done to allow Power LED (if installed).

When attaching the PCB to the frame (using M2 bolts), they should be very lightly
tightened. The screws are just to locate the PCB, leaving them loose will allow
The PCB to move, and improve sound quality.

### Bezel

The bezel has a different aesthetic, to the traditional TRS-80 bezel. 

Printing was done without supports, with the top of the bezel facing the build plate, 
this means you can achieve a pattern based on the texture of the build plate used.

The Bezel cannot be printed on a regular size 3d Printer,
and has been broken into 2 pieces using dowels to connect the 2 parts.

## Software

TODO Provided by Rev 1.4 ROM replacement.

Fork in GitHub repository. Todo 

## Matrix

Keyboard Matrix - PASTE HERE

## Limitations

* No dedicated @ Key, it has been removed replaced with Shift-2.
* Any software that provides its own KB driver, may have issues with the modified layout.
* Euro or British keys are not supported e.g. $ vs GBP point sign.

## Credits

* Marcus Erz for his MX keyboard design, which this project referenced during the design phase.
This includes the PCB design which this project used as a starting point. 

