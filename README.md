# CNFET-OCL
The CNFET-OCL project is to develop open source cell libraries for predictive sub-10nm carbon nanotube field effect transistor (CNFET) technology. CNFET7, the cell library for the 7nm CNFET technology, is now open and helps to design various combinational and sequential circuits by combining with EDA tools. CNFET7 is built with the VS-CNFET model developed by the Nanoelectronics Lab in Stanford University and well reproduces the cell library used in the state-of-the-art research work that designs the OpenSPARC T2 processor with CNFETs. For more details on CNFET7, see our ASP-DAC'23 paper.

## Usage
Liberyty file is used in Cadence Genus to do synthesis and if you want to use Design Compiler to do some synthesis jobs, please use Library compiler to transfer .lib to .db. 

LEF files and qrctechfile are used in Cadence Innovus and Quantus for P&R and Parasitic extraction.
Place and route are not supported in Synopsys tools, only in Cadence Innovus.

The qrctechfile is compressed because it is too large, so please use the following command to decompress it before using:

gzip -d *.gz

If you have Synopsys StarRC, you can also use the Nxtgrd file to do parasitic extraction with the LEF files and DEF file after P&R.

If you use our cell library in any published work, we would appreciate a citation for the following paper.

- C. Shi, S. Miwa, T. Yang, R. Shioya, H. Yamaki, and H. Honda, CNFET7: An Open Source Cell Library for 7-nm CNFET Technology, In Proceedings of the 28th Asia and South Pacific Design Automation Conference (ASP-DAC) (to appear)

If you have any questions or problems, please contact cnfet@hpc.is.uec.ac.jp.
