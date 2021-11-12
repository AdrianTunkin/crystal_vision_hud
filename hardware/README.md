# CRYSTAL VISION HUD
### Head-Up Display (HUD) System for safe driving


Crystal Vision is a portable Head-Up Display (HUD) system that projects an image on the windshield of your car. 
Both the driver and the passengers see it as a semi-transparent image that “levitates” over the hood of the car.

#### Copyright (C) 2015-2018, Crystal Vision Ltd.

Hardware directory contains hardware schematics, design sources, and revision changes.

![image](https://user-images.githubusercontent.com/49099551/141489558-030077ef-66f4-4935-9c06-759f7649cf16.png)


The Crystal Vision HUD electronic board is 6 layer PCB.

![Crystal-HUD PCB](https://user-images.githubusercontent.com/49099551/141488930-c96052b2-1ed0-468a-831e-c55ef6960721.png)


### Hardware revision changes log:

#### Hardware revision 1.0

* initial release

#### Hardware revision 1.1

* 1. Adjusted white print of label
* 2. Added bypass near FET2
* 3. Added white print for the UART connector at the bottom of the board
* 4. Fixed white print of R106 and R116
* 5. R29 placed a bit further from C84

#### Hardware revision 2.0

* 1. Changed from eMMC 4GB 1.00mm pitch to eMMC  16GB 0.50mm pitch.
* 2. C212 and C213 were increased to 33pF and to 0402.
* 3. R66 value changed from NA(0R) to NA(22R)
* 4. RM15's package changed from RA1206_(4X0603)_4B8_22R to RA0805_(4X0402)_22R as component optimisation.
* 5. C119 and VR1 changed from PTH to SMT type in the KiCad settings. In reallity, C119 and VR1 did not change. 
* 6. PWRLED1 and CHGLED1 labels corrected in the white print.
* 7. WP_Enable1 jumper added to the SPI_Flash.
* 8. U4 changed from NA(H27UBG8T2BTR-BC(TSOP48)) to NA(MT29F64G08CBABA-WP(TSOP48)), i.e. when populated 8GB NAND instead of 4GB.


#### Hardware revision 2.1

* 1. eMMC KLMAG2GEND-B031(FBGA153)(16G) changed with new eMMC KLMAG1JETD-B041(FBGA153)(16G)

#### Hardware revision 2.2

* 1. Added R62(10k/0402) pull-down to the eMMC's data strobe line;
* 2. RM14, RA0805_(4X0402)_22R replaced by 4 resistors 22R/0402, i.e. R121-R124;
* 3. R73[NA(22R/0402)] was added to enable SPI0 software CS option to the UEXT via PH10, when the SPI_Flash is populated.
* 4. L9 was changed from 2.7nH/L0402 to NA(2.7nH/L0402), and C88 from 24pF to NA(24pF);
* 5. MIPI-DSI1 changed: MIPI-DSI1 connector's pinout completely changed for Raspberry-Pi compatability; added the resistors: R125 to R132;
* 6. In the DRC drill to drill clerance was set to 12mils and all related errors were corrected;
* 7. UEXT1 was changed from NA(HN2x5) to HN2x5;
* 8. All 3Ds were assigned;
* 9. It was added C94(NA/0402) to the eMMC's clock line just in case;
* 10. NAND and related components removed forever;
* 11. In the schematic all "/" signs were exchanged with "\";
* 12. Improvements around the placement of a number of resistors related to the PHY signals to reduce EMI emissions;
* 13. Added U4 EEPROM - AT24C16C-SSHM-T(SOIC-8_150mil) and also C39, 100nF/10V/10% to the UEXT's I2C to avoid conflict with the same EEPROM
* 14. R15[NA(22R/R0402)] added in serial to the eMMC's datastrobe signal to be able to disconnect when no HS400 mode or to add a serial filter to reduce EMI;
* 15. U2 and U3's packages improved;


#### Hardware revision 2.3

* 1. Added antenna ANT2(NA(U.FL-R-SMT-1)), R16(0R) and R17(NA/0R);
* 2. Removed FB1(FB0402/PZ1005U601-R45TF-1) and FB2(FB0402/PZ1005U601-R45TF-1) and placed R18(22R/0402) and R19(22R/0402) resistors instead.;
* 3. Adjusted the lengths of some eMMC wires;
* 4. C93 changed from 24pF to 24pF\50V/5%. C88 and C198 changed from NA/24pF to NA(24pF\50V/5%);
* 5. Changing 5.1 eMMC at 3.3V (up from 1.8V operation) for better reliability, PWR_PC1 jumper has to be set to position 1-2 for 3.3V operation.



