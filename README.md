# Handmade KiCAD libraries
Custom KiCAD symbols, footprints and 3D models.

## Symbols
* Display_Graphic_Homemade.lib
    * [SSD1306](https://cdn-shop.adafruit.com/datasheets/SSD1306.pdf): Monochrome 0.96" OLED Graphics Display 128x64px, I2C 3.3V to 5V VDD.
* Keypad_Homemade.lib
    * [KEYPAD3X4](https://media.digikey.com/pdf/Data%20Sheets/Adafruit%20PDFs/1824_Web.pdf): Any keypad with 3 columns and 4 rows.
    * [KEYPAD4X4](https://www.parallax.com/sites/default/files/downloads/27899-4x4-Matrix-Membrane-Keypad-v1.2.pdf): Any keypad with 4 columns and 4 rows.
* Power_Management_Homemade.lib
    * [TPS22960](http://www.ti.com/lit/ds/symlink/tps22960.pdf): 2-ch, 1.62 V to 5.5 V, 0.5A, 435mΩ load switch with output discharge.
* Relay_Homemade.lib
    * SPDT_RELAY: Generic SPDT relay. SPDT (Single pole double throw) means it can switch one input terminal 
    between two output terminals.
* Sensor_Gas_Homemade.lib
    * [PPD42](https://www.mouser.com/datasheet/2/744/Seeed_101020012-1217636.pdf): Optical air quality sensor. 
    Measures the particulate matter level in air by counting Low Pulse Occupancy time.

## Footprints
* Connector_Fischertechnik_Homemade.pretty
    * Barrel_Connector_THT_D9mm_Drill7mm: 
    Fischertechnik produces some [nice training models](https://www.fischertechnik.de/en/products/simulating/training-models)
    that look essentially like an industry automation piece in miniature.
    We used those to [teach students industrial programming](https://www.shortn0tes.com/2017/04/make-interface-board-to-connect.html).
    The connectors that hardware from these kits use look like
    [a tiny metal stick](https://content.ugfischer.com/cbfiles/fischer/Zulassungen/ft/37783-Mini-switch.pdf),
    and I needed to interface them to my PCB.
    Turns out an ordinary jeans rivet can act as a receptable
    for them, and can be soldered on PCBs! Footprint in question can accept
    exactly this kind of rivet, hole diameter is 7mm.
* Connector_KEFA_Homemade.pretty
    * [KF250-[N]pin](http://en.cnkefa.com/index.php?c=product&id=221): Through hole spring cage connector,
    1x2, 1x3, 1x7 and 1x20, 3.5mm pitch.
    * [KF141V-6P_P2.54mm](http://en.cnkefa.com/index.php?c=product&id=212): Through hole spring cage connector,
    1x06, 2.54mm pitch, double row with pin pairs internally connected in a column.
* Relay_THT_Homemade.pretty
    * [HUIKE_HK4100F](https://img.ozdisan.com/ETicaret_Dosya/445413_4369639.pdf):
    Subminiature signal relay, SPDT, 3A switching capability, 5V coil
    * [SANYOU_SRD](http://www.sanyourelay.ca/public/products/pdf/SRD.pdf):
    Sanyou SRD series. Miniature Power Relay, SPDT, ex.: SRD-S-112D
* Symbol_Homemade.pretty
    * Barrel_Jack_Positive_Center_Silkscreen: Silkscreen on top. Show the barrel jack polarity
    simply on the PCB itself! 
    * Rotation_[C]CW_Silkscreen: Silkscreen on top. You can use this e.g. to indicate that the motor connected
    to these terminals is supposed to rotate in a specific direction.

## 3D Models
Most models correspond to the footprint in the same directory under `footprints/`,
unless noted otherwise.

There's an STL file provided with each WRL/STEP model -
this is just for convenience. You can preview those in most modern
operating systems.

* Connector_Fischertechnik_Homemade.3dshapes
    * Barrel_Connector_THT_D9mm_Drill7mm
* Connector_KEFA_Homemade.3dshapes
    * KF250-[N]pin

