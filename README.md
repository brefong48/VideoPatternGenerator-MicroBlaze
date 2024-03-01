# VideoPatternGenerator-MicroBlaze
 The Video Pattern Generator project is a system that generates and displays a variety of
 test patterns on a VGA monitor for testing purposes. This design integrates key components,
 including Xilinx Artix-7 FPGA, a MicroBlaze soft-core processor for system control, two
 external memory ICs to clock the processor, a VGA interface for synchronization control, and a
 user interface utilizing a push button from the Basys 3 board. The 32-bit MicroBlaze processor
 will manage all the key components of the generator. The two parallel external memory ICs are
 the Cypress CY7C1049G30-10VXI (SRAM) and the Spansion S29AL008J70BFI023 (NOR
 Flash memory). The VGA interface ensures that the system generates video output signals to go
 with the VGA synchronization parameters for the 640x480 pixels with a 60 MHz refresh rate.
 Finally, the user interface provides an opportunity for the user to change the test patterns using
 the push button.
 I have gathered the evidence and calculations that the MicroBlaze will need to de-rate its
 timing to ensure the seamless operation of the Video Pattern Generator. The code will be written
 in Verilog and tested in Vivado and SDK. This report will incorporate three Worse-Case
 Analyses for the Artix-7 FPGA and the two external memory ICs. Testing and validation will be
 undertaken, considering the complexities of adding two additional memories to the processor and
 FPGA.
