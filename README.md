# CNFET-OCL
The CNFET-OCL project is to develop open source cell libraries for predictive sub-10nm carbon nanotube field effect transistor (CNFET) technology. CNFET7, the cell library for the 7nm CNFET technology, is now open and helps to design various combinational and sequential circuits by combining with EDA tools. CNFET7 is built with the VS-CNFET model developed by the Nanoelectronics Lab in Stanford University and well reproduces the cell library used in the state-of-the-art research work that designs the OpenSPARC T2 processor with CNFETs. For more details on CNFET7, see our ASP-DAC'23 paper.

## Descriptions
CNFET7 includes the following files.
- Two Liberty files (CCS and NLDM)
- Two LEF files (Cell and Tech)
- Two QRC files
- A Nxtgrd file

The Liberty files can be read from Cadence Genus directly. If you would like to use Design Compiler for logic synthesis, please use Library Compiler to transfer a .lib file to a .db file. 

The LEF and QRC files are used in Cadence Innovus and Quantus for P&R and parasitic extraction, respectively. Our cell library does not support P&R with Synopsys tools at present. QRC file has two versions, one is generated with regular dieletric constant, the other one is generated with a low K(K=2.5) assumption. Because the QRC file is compressed with gzip, the decompression is needed before use. For the decompression, you move to the QRC dierectory and then type the following command.

gzip -d *.gz

If you have Synopsys StarRC, you can also use the Nxtgrd file for parasitic extraction with LEF and DEF files after P&R. The Nxtgrd file was generated with regular dieletric constant.

## Related publication
If you use our cell library in any published work, we would appreciate a citation for the following paper.

- C. Shi, S. Miwa, T. Yang, R. Shioya, H. Yamaki, and H. Honda, CNFET7: An Open Source Cell Library for 7-nm CNFET Technology, In Proceedings of the 28th Asia and South Pacific Design Automation Conference (ASP-DAC) (to appear)

## License
Our cell library has a BSD 3-Clause license.

## Contact
If you have any questions or problems, please contact cnfet@hpc.is.uec.ac.jp.
