Day wise Detailed Lab Documentation

Day 1 
2:1 Multiplexer RTL to Gate Level Mapping
Designed a 2:1 multiplexer and synthesized it using Yosys. Generated the gate level netlist using the SKY130 standard cell library. The module good mux consists of inputs i0 i1 sel and output y. Verified mapping to the standard cell mux2 1. Studied internal wire connections and assign statements. Analyzed the synthesized schematic where inputs are buffered for signal strength and output is buffered before final assignment. Confirmed correct conversion from RTL to structural hardware.

Day 2 
Hierarchical Design Mapping and Flattening
Worked on hierarchical design using multiple modules including sub module 1 and sub module 2. Sub module 1 performs AND operation and sub module 2 performs OR operation. Verified that the design is purely combinational with no memory elements. Performed hierarchy checking and technology mapping using Yosys. Observed mapping to SKY130 standard cells such as AND and OR gates. Applied flattening to remove hierarchy and merge all modules into a single level design. Observed optimized signal flow and removal of unused modules. Also analyzed individual sub module synthesis.

Day 3 
Optimization Flip Flops and Constant Propagation
Implemented combinational logic including two input AND two input OR three input AND and XNOR. Observed drive strength selection buffer insertion and handling of unused inputs.
Studied sequential circuits including asynchronous reset flip flop asynchronous set flip flop and synchronous reset flip flop. Verified behavior using waveform simulation. Observed that asynchronous reset works independent of clock while synchronous reset depends on clock. Verified mapping to standard cells such as D flip flop and clock inverter.
Studied constant propagation cases where input is fixed. Observed that unnecessary flip flops are removed and logic is simplified. In some cases the circuit becomes purely combinational. Also analyzed pipeline behavior in cascaded flip flops.
Studied arithmetic optimization where multiplication by constants is implemented using shift operations.
Designed and analyzed counter circuits including simple and optimized multi bit counters. Observed feedback loops and use of combinational logic for next state generation.

Day 4 
Multiplexer and Coding Behavior
Designed a correct multiplexer using ternary operator and verified correct waveform behavior. Observed that synthesis may implement logic using gates instead of a direct multiplexer cell.
Analyzed an incorrect multiplexer design and observed wrong output behavior due to faulty RTL logic.
Studied blocking assignment behavior and observed sequential execution inside always block. Compared simulation behavior with synthesized hardware and understood the importance of using non blocking assignments in sequential logic.

Day 5 
Latch Inference Case Statements and Advanced Designs
Designed a circuit with incomplete if condition and observed latch inference. The output holds previous value leading to memory behavior. Learned importance of complete conditional statements.
Implemented case statement and observed its conversion into decoder logic followed by multiplexer structure. Verified correct functionality.
Observed partial latch behavior where latch exists in one signal path but not in another.
Designed advanced circuits including multiplexer using loop four input multiplexer eight output demultiplexer using case and generate methods and ripple adder.
Verified all designs using waveform simulation and confirmed correct timing behavior.

Conclusion
Successfully completed all labs covering RTL design synthesis and verification. Understood the complete design flow from RTL to gate level implementation. Explored combinational logic sequential circuits optimization techniques and common coding issues such as latch inference and blocking assignments. All designs were verified using simulation and mapped to SKY130 standard cells.
