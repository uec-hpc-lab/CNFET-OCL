# CNFET-OCL
Open Source Cell Library for Predictive CNFET Technology

CNFET7 is an open-source 7-nm CNFET (Carbon nanotube field-effect transistor) Cell library based on the VS-CNFET model of Stanford University and supports Cadence APR flow.

Liberyty file is used in Cadence Genus to do synthesis and if you want to use Design Compiler to do some synthesis jobs, please use Library compiler to transfer .lib to .db. 

LEF files and qrctechfile are used in Cadence Innovus and Quantus for P&R and Parasitic extraction.
Place and route are not supported in Synopsys tools, only in Cadence Innovus.

The qrctechfile is compressed because it is too large, so please use the following command to decompress it before using:

gzip -d *.gz

If you have Synopsys StarRC, you can also use the Nxtgrd file to do parasitic extraction with the LEF files and DEF file after P&R.

If you use the CNFET7 cell library in any published work, we will feel thanksful for a citation of this paper:

C. Shi, S. Miwa, T. Yang, R. Shioya, H. Yamaki, and H. Honda, CNFET7: An Open Source Cell Library for 7-nm CNFET Technology, The 28th Asia and South Pacific Design Automation Conference (ASP-DAC) 







