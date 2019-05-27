
Copyright (c) 2018 Group of Computer Architecture.
All Rights Reserved.

This directory includes an executable of our tool PolyCleaner. For details on the techniques behind see the publication "PolyCleaner: Clean your Polynomials before Backward Rewriting to Verify Million-gate Multipliers" by Alireza Mahzoon, Daniel Große, and Rolf Drechsler accepted at ICCAD 2018.

PolyCleaner was developed and tested in Fedora 24. For related information, e.g. other SCA-based verification approaches, please visit http://www.sca-verification.org/ or contact polycleaner@sca-verification.org.


*************************************************


Use the following command to verify multiplier:

	./PolyCleaner <inputFile> <outputFile>


inputFile:  name of a gate-level Verilog file to read

outputFile: name of output file containing verification data
