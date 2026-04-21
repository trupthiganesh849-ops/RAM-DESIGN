# RAM-DESIGN
*COMPANY*: CODTECH IT SOLUTIONS
*NAME*: TRUPTHI GANAPATI NAIK
*INTERN ID*: CTIS7707
*DOMAIN*: VLSI DURATION : 4 WEEKS
*MENTOR*: NEELA SANTOSH


## Description 
A simple synchronous single-port Random Access Memory (RAM) module with read and write operations has been designed and simulated using SystemVerilog. RAM is an essential component in digital systems, used for temporary storage of data that can be accessed randomly using address lines. In this design, the RAM operates synchronously, meaning that all read and write operations are controlled by a clock signal, ensuring stable and predictable behavior.
The RAM module is parameterized to make it flexible and reusable. Two important parameters are defined: DATA_WIDTH and ADDR_WIDTH. The DATA_WIDTH determines the number of bits stored in each memory location, which is set to 8 bits in this design. The ADDR_WIDTH specifies the number of address lines, set to 4 bits, allowing access to 2⁴ = 16 memory locations. This parameterization allows the size of the memory to be easily modified without changing the internal logic of the design.
The module consists of inputs and outputs such as the clock signal (clk), write enable signal (we), address input (addr), data input (din), and data output (dout). Internally, a memory array is declared using a register array that stores multiple data values. Each memory location can hold an 8-bit value, and the total number of locations is determined by the address width.
The core functionality of the RAM is implemented using an always block that is triggered on the positive edge of the clock signal (posedge clk). This ensures that all operations occur synchronously with the clock. When the write enable signal (we) is high, the RAM performs a write operation, storing the input data (din) into the memory location specified by the address (addr). When the write enable signal is low, the RAM performs a read operation, and the data stored at the specified address is assigned to the output (dout). This design ensures that both read and write operations are controlled and occur only at clock edges.
To verify the functionality of the RAM, a testbench is developed. The testbench generates a clock signal and applies a sequence of inputs to the RAM module. Initially, it writes known data values such as “aa”, “bb”, “cc”, and “dd” into consecutive memory locations. After completing the write operations, the testbench reads the data from the same addresses. The results are displayed using print statements, allowing verification of correctness.
The simulation results show that the data read from each address matches the data that was previously written. For example, the output displays “Read Addr 0: aa”, “Read Addr 1: bb”, “Read Addr 2: cc”, and “Read Addr 3: dd”. This confirms that both write and read operations are functioning correctly, and the RAM behaves as expected.
The design and simulation were carried out using EDA Playground, which is an online platform for writing and testing hardware description language (HDL) code such as Verilog and SystemVerilog. The simulation tool used within EDA Playground is Icarus Verilog, which compiles and executes the code. The platform also supports waveform viewing using EPWave, which helps in analyzing signal transitions over time.
In conclusion, the synchronous RAM module has been successfully designed, tested, and verified. The use of a clock signal ensures reliable operation, and the parameterized design makes it adaptable for different memory sizes. The correct simulation output demonstrates that the RAM performs accurate read and write operations, making it a fundamental building block for more complex digital systems.

# Output
<img width="1240" height="475" alt="Image" src="https://github.com/user-attachments/assets/e3d56127-5657-4c8a-98c3-7e4bcd0d5830" />
