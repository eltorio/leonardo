# Leonardo
Arduino Leonardo schematic ported to Kicad

# Kicad 8
The design has been ported to Kicad 8.  
* DRC shows no error nor warning on PCB.
* All selected parts are easily availables.
* All parts contains 3 additional fields
    * Manufacturer containing the name of the manufacturer
    * Manufacturer_ref containing the part real reference
    * Digikey_ref containing a Digikey part number

NM, DNP parts are parts not mounted

# Why
Because I need to adapt the Leonardo design to include other functionalities my first work is to port the very good Arduino Leonardo rev3d to Kicad 6.  

# Crystal
16MHz Crystal is not yet selected…

# Schematic
[![Schematic](https://raw.githubusercontent.com/eltorio/leonardo/main/schematic.png)](https://github.com/eltorio/leonardo/raw/main/schematic.pdf?raw=true)

# Board
![Board](https://github.com/eltorio/leonardo/blob/main/board.png?raw=true)
The board is adapted and routed with the parts I have selected.  
Kicad 8 DRC check doesn't show any errors nor any warning.  
Component references are hidden by default to match the Arduino Leonardo silkscreen. If you need the references, use the [Hide References plugin](https://github.com/joelsa/kicad-hide-references-plugin) which can be easily installed via the Plugin and Content Manager.

# 3D Render

## Without component references
![Front without component references](https://raw.githubusercontent.com/eltorio/leonardo/main/board_3d_front.png?raw=true)

## With component references
![Front with component references](https://raw.githubusercontent.com/eltorio/leonardo/main/board_3d_front_w_ref.png?raw=true)

# BOM
The [BOM](https://raw.githubusercontent.com/eltorio/leonardo/main/Leonardo_Rev3e.html) was automatically generated with [python/bom.py](https://github.com/eltorio/leonardo/blob/main/python/bom.py) add this script in the BOM dialog.  
The html BOM was converted to MarkDown with https://www.convertsimple.com/convert-html-to-markdown/   

[comment]: <> (generated from html bom with https://www.convertsimple.com/convert-html-to-markdown/)  
**Component Count: 56**

| Ref | Qnty | Value | Footprint | Datasheet | Manufacturer | Manufacturer_ref | Digikey_ref |
| --- | --- | --- | --- | --- | --- | --- | --- |
| C1, C2, C6, C9, C13, C22 | 6   | 100n | Leonardo_Rev3e:C0603-ROUND | [link](https://connect.kemet.com:7667/gateway/IntelliData-ComponentDocumentation/1.0/download/datasheet/C0603C104J4RACTU) | Kemet | C0603C104J4RAC7867 | [399-C0603C104J4RAC7867CT-ND](https://www.digikey.com/en/products?mpart=399-C0603C104J4RAC7867CT-ND) |
| C3, C4 | 2   | 22p | Leonardo_Rev3e:C0603-ROUND | [link](https://connect.kemet.com:7667/gateway/IntelliData-ComponentDocumentation/1.0/download/datasheet/C0603C220K5RAC7867) | Kemet | C0603C220K5RAC7867 | [399-14962-1-ND](https://www.digikey.com/en/products?mpart=399-14962-1-ND) |
| C5, C7, C11, C14 | 4   | 1uF | Leonardo_Rev3e:C0603-ROUND | [link](https://connect.kemet.com:7667/gateway/IntelliData-ComponentDocumentation/1.0/download/datasheet/C0603C105K4RAC7411) | Kemet | C0603C105K4RAC7411 | [399-C0603C105K4RAC7411CT-ND](https://www.digikey.com/en/products?mpart=399-C0603C105K4RAC7411CT-ND) |
| C8, C10, C12 | 3   | 10u | Leonardo\_Rev3d:SMC\_B | [link](https://api.kemet.com/component-edge/download/datasheet/T491B106M016AT.pdf) | Kemet | T491B106M016AT | [399-3708-1-ND](https://www.digikey.com/en/products?mpart=399-3708-1-ND) |
| D1  | 1   | M7  | Leonardo_Rev3e:SMB |     |     |     |     |
| D2  | 1   | 1N4148W-TP | Leonardo_Rev3e:MINIMELF | [link](https://www.mccsemi.com/pdf/Products/1N4148W(SOD-123).pdf) | MCC | 1N4148W-TP | [1N4148WTPMSCT-ND](https://www.digikey.com/en/products?mpart=1N4148WTPMSCT-ND) |
| D+0 | 1   | DNP | Leonardo_Rev3e:TP-1.00MM |     |     |     |     |
| D-0 | 1   | DNP | Leonardo_Rev3e:TP-1.00MM |     |     |     |     |
| EXTPOWER0 | 1   | POWERSUPPLY_DC21MMX | Leonardo\_Rev3d:POWERSUPPLY\_DC-21MM |     |     |     |     |
| F1  | 1   | MF-MSMF050-2 500mA | Leonardo_Rev3e:L1812 | [link](https://www.bourns.com/docs/product-datasheets/mf-msmf.pdf) | Bourns | MF-MSMF050-2 | [MF-MSMF050-2CT-ND](https://www.digikey.com/en/products?mpart=MF-MSMF050-2CT-ND) |
| FID1, FID2, FID3 | 3   | DNP | Leonardo_Rev3e:FD-1-1.5 |     |     |     |     |
| GND0 | 1   | DNP | Leonardo_Rev3e:TP-1.00MM |     |     |     |     |
| IC1 | 1   | REG1117-5 | Leonardo_Rev3e:SOT223 | [link](https://www.ti.com/lit/gpn/reg1117) | TI  | REG1117-5 | [REG1117-5-ND](https://www.digikey.com/en/products?mpart=REG1117-5-ND) |
| IC2 | 1   | LMV358IDGKR | Leonardo_Rev3e:MSOP08 | [link](https://www.ti.com/lit/gpn/lmv358) | TI  | 296-13455-1-ND | [LMV358IDGKR](https://www.digikey.com/en/products?mpart=LMV358IDGKR) |
| ICSP0 | 1   | ICSP | Leonardo_Rev3e:2X03 | [link](https://www.te.com/commerce/DocumentDelivery/DDEController?Action=srchrtrv&DocNm=146486&DocType=Customer+Drawing&DocLang=English) | TE  | 5-146486-3 | [A128860-ND](https://www.digikey.com/en/products?mpart=A128860-ND) |
| J1  | 1   | USBMICRO | Leonardo_Rev3e:10118194-0001LF | [link](https://www.amphenol-cs.com/media/wysiwyg/files/drawing/10118194.pdf) | Amphenol | 10118194-0001LF | [609-4618-1-ND](https://www.digikey.com/en/products?mpart=609-4618-1-ND) |
| J2, J3 | 2   | 8x1F-H8.5 | Leonardo_Rev3e:1X08 | [link](https://media.digikey.com/pdf/Data%20Sheets/Sullins%20PDFs/Female_Headers.100_DS.pdf) | Sullins | PPPC081LFBN-RC | [S7041-ND](https://www.digikey.com/en/products?mpart=S7041-ND) |
| J4  | 1   | 6x1F-H8.5 | Leonardo_Rev3e:1X06 | [link](https://media.digikey.com/pdf/Data%20Sheets/Sullins%20PDFs/Female_Headers.100_DS.pdf) | Sullins | PPPC061LFBN-RC | [S7039-ND](https://www.digikey.com/en/products?mpart=S7039-ND) |
| JP1 | 1   | 10x1F-H8.5 | Leonardo_Rev3e:1X10 | [link](https://media.digikey.com/pdf/Data%20Sheets/Sullins%20PDFs/Female_Headers.100_DS.pdf) | Sullins | PPPC101LFBN-RC | [S7043-ND](https://www.digikey.com/en/products?mpart=S7043-ND) |
| JP2 | 1   | OTG | Leonardo\_Rev3d:HEADER\_2_2.54 | [link](~) | Samtex | DW-02-07-T-S-200 | [SAM15134-ND](https://www.digikey.com/en/products?mpart=SAM15134-ND) |
| L0  | 1   | Yellow | Leonardo\_Rev3d:CHIPLED\_0805 | [link](https://optoelectronics.liteon.com/upload/download/DS22-2000-110/LTST-C171KSKT.pdf) | Lite-on | LTST-C171KSKT | [160-1428-1-ND](https://www.digikey.com/en/products?mpart=160-1428-1-ND) |
| L1, L2 | 2   | MH2029-300Y | Leonardo_Rev3e:0805 | [link](https://www.bourns.com/docs/Product-Datasheets/mh.pdf) | Bourns | MH2029-300Y | [MH2029-300YCT-ND](https://www.digikey.com/en/products?mpart=MH2029-300YCT-ND) |
| ON0 | 1   | Green | Leonardo\_Rev3d:CHIPLED\_0805 | [link](https://optoelectronics.liteon.com/upload/download/DS22-2000-110/LTST-C171KSKT.pdf) | Lite-on | LTST-C171KGKT | [160-1426-1-ND](https://www.digikey.com/en/products?mpart=160-1426-1-ND) |
| R1  | 1   | 1M  | Leonardo_Rev3e:R0603-ROUND | [link](https://www.bourns.com/docs/product-datasheets/cr.pdf?sfvrsn=574d41f6_14) | Bourns | CR0603-FX-1004ELF | [CR0603-FX-1004ELFCT-ND](https://www.digikey.com/en/products?mpart=CR0603-FX-1004ELFCT-ND) |
| R2, R3 | 2   | NM  | Leonardo_Rev3e:R0402 |     |     |     |     |
| R4  | 1   | 10K | Leonardo_Rev3e:R0603-ROUND | [link](https://www.bourns.com/docs/product-datasheets/cr.pdf?sfvrsn=574d41f6_14) | Bourns | CR0603-FX-1002ELF | [CR0603-FX-1002ELFCT-ND](https://www.digikey.com/en/products?mpart=CR0603-FX-1002ELFCT-ND) |
| RESET0 | 1   | TS07-667-30-BK-160-SMT-TR | Leonardo_Rev3e:TS07 | [link](https://www.cuidevices.com/product/resource/ts07.pdf) | CUI | TS07-667-30-BK-160-SMT-TR | [2223-TS07-667-30-BK-160-SMT-TRCT-ND](https://www.digikey.com/en/products?mpart=2223-TS07-667-30-BK-160-SMT-TRCT-ND) |
| RN1 | 1   | 10K | Leonardo_Rev3e:CAY16 | [link](https://www.bourns.com/docs/Product-Datasheets/CATCAY.pdf) | Bourns | CAY16-1002F4LF | [CAY16-1002F4LFCT-ND](https://www.digikey.com/en/products?mpart=CAY16-1002F4LFCT-ND) |
| RN2 | 1   | 1K  | Leonardo_Rev3e:CAY16 | [link](https://www.bourns.com/docs/Product-Datasheets/CATCAY.pdf) | Bourns | CAY16-1001F4LF | [CAY16-1001F4LFCT-ND](https://www.digikey.com/en/products?mpart=CAY16-1001F4LFCT-ND) |
| RN3 | 1   | 22R | Leonardo_Rev3e:CAY16 | [link](https://www.bourns.com/docs/Product-Datasheets/CATCAY.pdf) | Bourns | CAY16-22R0F4LF | [CAY16-22R0F4LFCT-ND](https://www.digikey.com/en/products?mpart=CAY16-22R0F4LFCT-ND) |
| RX0 | 1   | Yellow | Leonardo\_Rev3d:CHIPLED\_0805 | [link](https://optoelectronics.liteon.com/upload/download/DS22-2000-110/LTST-C171KSKT.pdf) | Lite-on | LTST-C171KSKT | [160-1426-1-ND](https://www.digikey.com/en/products?mpart=160-1426-1-ND) |
| T1  | 1   | FDN340P | Leonardo_Rev3e:SOT-23 | [link](https://media.digikey.com/pdf/Data%20Sheets/UTD%20Semi%20PDFs/UMW%20FDN340P.pdf) | UMW | FDN340P | [4518-FDN340PCT-ND](https://www.digikey.com/en/products?mpart=4518-FDN340PCT-ND) |
| TX0 | 1   | Yellow | Leonardo\_Rev3d:CHIPLED\_0805 | [link](https://optoelectronics.liteon.com/upload/download/DS22-2000-110/LTST-C171KSKT.pdf) | Lite-on | LTST-C171KSKT | [160-1426-1-ND](https://www.digikey.com/en/products?mpart=160-1426-1-ND) |
| U1  | 1   | ATMEGA32U4-XUMU | Leonardo_Rev3e:QFN44ML7X7 | [link](http://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-7766-8-bit-AVR-ATmega16U4-32U4_Summary.pdf) | Microchip | ATMEGA32U4-MU | [ATMEGA32U4-MU-ND](https://www.digikey.com/en/products?mpart=ATMEGA32U4-MU-ND) |
| U2  | 1   | ATMEGA32U4-XUAU | Leonardo_Rev3e:TQFP44-PAD | [link](http://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-7766-8-bit-AVR-ATmega16U4-32U4_Summary.pdf) | Microchip | ATMEGA32U4-AU | [ATMEGA32U4-AU-ND](https://www.digikey.com/en/products?mpart=ATMEGA32U4-AU-ND) |
| U3  | 1   | LP2985-33DBVR | Leonardo_Rev3e:SOT23-DBV | [link](https://www.ti.com/lit/gpn/LP2985-N) | TI  | LP2985IM5-3.3 | [LP2985IM5-3.3CT-ND](https://www.digikey.com/en/products?mpart=LP2985IM5-3.3CT-ND) |
| VUSB0 | 1   | DNP | Leonardo_Rev3e:TP-1.00MM |     |     |     |     |
| Y1  | 1   | 16MHz KX-7 | Leonardo_Rev3e:CRYSTAL-3.2-2.5 |     |     |     |     |
| Z1, Z2 | 2   | CG0603MLC-05E | Leonardo\_Rev3d:CT\_CN0603 | [link](https://www.bourns.com/docs/product-datasheets/cga-mlc.pdf) | Bourns | CG0603MLC-05E | [CG0603MLC-05ECT-ND](https://www.digikey.com/en/products?mpart=CG0603MLC-05ECT-ND) |
