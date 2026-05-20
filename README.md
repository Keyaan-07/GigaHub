# GigaHub
GigaHub is a USB 3.0 Hub capable of speeds upto 5Gbps. It comes in a small form factor and can handle upto 4 devices simultaneously. The silkscreen on the bottom makes it obvious. You plug in the USB-C cable on one side, and you get 4x USB-C cables. 

I made this project just for fun and because i had some free time. I could've made USB 2.0 hub but this was a bit challenging thus i made this!!

![zine magazine page](/media/GigaHub.png)
![PCB](/media/usb-hub.png)
![3d](/media/usb-hub-3d-nobg.png)
![3d-back](/media/usb-hub-3d-back.png)
![schematic](/media/usb-hub-schematic.png)



# How to build
To Assemble this PCB, first you need to be familiar with soldering. You take your bare PCB, apply solder paste on it(soldering iron and solder is not recommended because it involves pins under the surface, such as the USB-C receptacles). Then, you take a hotplate or a hot air gun and melt the solder appropriately. There are many tutorials online teaching it in a great way, go search there!

The linked html file under /hardware/bom helps you with placement!

# BOM
|Designator                                                  |Function         |Value           |Footprint                                        |Quantity         |Price |Amount |Order|Note      |Link                                              |
|------------------------------------------------------------|-----------------|----------------|-------------------------------------------------|-----------------|------|-------|-----|----------|--------------------------------------------------|
|PCB                                                         |PCB              |4 layer board   |49.57mm x 34.54mm                                |5                |0.4   |2      |Yes  |          |https://jlcpcb.com/                               |
|C1, C10, C11, C2, C3, C4, C5, C6, C7, C8, C9                |Capacitor        |100n            |402                                              |11               |0.0077|0.0847 |No   |          |https://www.lcsc.com/product-detail/C426067.html  |
|C12, C13                                                    |Capacitor        |15p             |402                                              |50               |0.019 |0.95   |Yes  |50 is MOQ |https://www.lcsc.com/product-detail/C441742.html  |
|J1, J2, J3, J4, J5                                          |Receptacle       |USB_C_Receptacle|USB_C_Receptacle_Molex_105450-0101               |5                |0.29  |1.45   |Yes  |          |https://www.lcsc.com/product-detail/C48887178.html|
|R1                                                          |Resistor         |9.53k           |402                                              |100              |0.0008|0.08   |Yes  |100 is MOQ|https://www.lcsc.com/product-detail/C96273.html   |
|R2, R3, R4, R10, R11, R12, R13, R14, R15, R16, R17, R18, R19|Resistor         |5.1k            |402                                              |13               |0.0056|0.0728 |No   |          |https://www.lcsc.com/product-detail/C278598.html  |
|R5                                                          |Resistor         |10k             |402                                              |100              |0.0006|0.06   |Yes  |100 is MOQ|https://www.lcsc.com/product-detail/C3020235.html |
|R6                                                          |Resistor         |90.9k           |402                                              |100              |0.0006|0.06   |Yes  |100 is MOQ|https://www.lcsc.com/product-detail/C2998102.html |
|R7                                                          |Resistor         |1M              |402                                              |100              |0.0009|0.09   |Yes  |100 is MOQ|https://www.lcsc.com/product-detail/C138033.html  |
|R8, R9                                                      |Resistor         |30k             |402                                              |100              |0.0007|0.07   |Yes  |100 is MOQ|https://www.lcsc.com/product-detail/C2909347.html |
|U1                                                          |Hub Controller IC|TUSB8041        |QFN-64-1EP_9x9mm_P0.5mm_EP6x6mm_ThermalVias      |1                |4.83  |4.83   |Yes  |          |https://www.lcsc.com/product-detail/C544686.html  |
|U2, U3                                                      |Power switch     |TPS2561         |VSON-10-1EP_3x3mm_P0.5mm_EP1.65x2.4mm_ThermalVias|2                |0.8   |1.6    |Yes  |          |https://www.lcsc.com/product-detail/C140303.html  |
|Y1                                                          |Crystal          |24 MHz          |Crystal_SMD_3225-4Pin_3.2x2.5mm                  |10               |0.036 |0.36   |Yes  |10 is MOQ |https://www.lcsc.com/product-detail/C41383243.html|
|                                                            |                 |                |                                                 |Shipping fee JLC |      |7.72   |     |          |                                                  |
|                                                            |                 |                |                                                 |Shipping fee LCSC|      |3.92   |     |          |                                                  |
|                                                            |                 |                |                                                 |Handling Fee LCSC|      |3      |     |          |                                                  |
|                                                            |                 |                |                                                 |Total            |      |26.3475|     |          |                                                  |
