
The Verilog files in this directory result from running Yosys [1] to convert the AOKI benchmarks [2] to a flattened gate-level Verilog netlist.

The files are named according to the schemata:

	SIZE-STAGE1_STAGE2_STAGE3


SIZE:	Input bit size of multiplier (16bit means that the design multiplies two 16bit numbers, i.e. 16*16)


STAGE1:	The type of first multiplier stage (partial product generator)
	
	SP: unsigned simple partial product generator
	BP: unsigned Booth partial product generator


STAGE2:	The type of second multiplier stage (partial product accumulator)
	
	AR: Array 
	CT: Compressor tree
	DT: Dadda tree
	WT: Wallace tree


STAGE3:	The type of third multiplier stage (final stage adder)
	
	RC: Ripple carry adder
	BK: Brent-Kung adder
	LF: Lander-Fischer adder
	CL: Carry look-ahead adder



References:
[1] Clifford Wolf. Yosys open synthesis suite. http://www.clifford.at/yosys/
[2] Arithmetic module generator based on acg. http://www.aoki.ecei.tohoku.ac.jp/arith/
