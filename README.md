# FPGA-Digital-Stopwatch-Countdown-Timer
FPGA-Based Digital Stopwatch with Countdown Timer

1. Project Overview

The FPGA-Based Digital Stopwatch with Countdown Timer is a digital electronics mini project developed using Verilog Hardware Description Language (HDL). It combines a stopwatch that counts upward and a countdown timer that counts downward.

The project demonstrates fundamental digital design concepts such as clock division, counters, control logic, finite-state machines, and seven-segment display decoding.

The design can be tested through RTL simulation using AMD Xilinx Vivado or a compatible Verilog simulator. With a suitable FPGA development board, it can also be implemented as a hardware project.

2. Objectives

- Design a digital stopwatch using Verilog HDL.
- Develop a countdown timer with a preset starting time.
- Implement Start, Pause, Reset, and Mode Select functions.
- Display time using seven-segment display logic.
- Verify circuit behavior using simulation waveforms.
- Understand FPGA-based digital system design.

3. Features

- Stopwatch mode: counts upward.
- Countdown mode: counts downward.
- Start and Pause controls.
- Reset functionality.
- Mode selection between stopwatch and countdown.
- Seven-segment display decoder.
- RTL simulation and waveform verification.
- Optional FPGA hardware implementation.

4. Technologies Used

- Hardware Description Language: Verilog HDL
- Design and Simulation Software: AMD Xilinx Vivado
- Alternative Online Simulator: EDA Playground
- Design Platform: FPGA
- Application Area: Digital Electronics and VLSI

5. Block Diagram

Clock Input
↓
Clock Divider
↓
Control Logic
↓
Stopwatch Counter / Countdown Counter
↓
Seven-Segment Decoder
↓
Digital Time Display

The control logic manages the operating mode and timer controls.

6. Working Principle

Stopwatch Mode

When the Start control is activated, the stopwatch counts upward at one-second intervals. Pause holds the current value, and Reset returns the counter to zero.

Example:

"00:00 → 00:01 → 00:02 → 00:03 → ..."

Countdown Mode

The countdown timer starts from a preset value and decreases at one-second intervals. When the timer reaches zero, it stops automatically.

Example:

"00:10 → 00:09 → 00:08 → ... → 00:01 → 00:00"

Seven-Segment Display

The display logic converts the numerical time digits into segment patterns so the current time can be shown on a seven-segment display.


7. Software Implementation

1. Create a project in Vivado or open an online Verilog simulator.
2. Write the Verilog source modules.
3. Create a testbench to generate the clock and apply control inputs.
4. Run behavioral simulation.
5. Verify the counter values and control behavior in the waveform.
6. Save a screenshot of the simulation results.
7. For hardware implementation, synthesize the design and configure the correct FPGA pins for the selected development board.

For faster simulation, a reduced clock-divider value can be used in the testbench.

8. Expected Results

Test case| Expected output
Reset| Timer returns to its reset value
Start stopwatch| Time increases
Pause| Current value is held
Resume| Counting continues
Start countdown| Time decreases
Countdown reaches zero| Timer stops
Mode selection| Selected timing mode becomes active

These are expected behaviors to verify during simulation.

9. Applications

- Sports and practice timing
- Laboratory experiments
- Examination countdown systems
- Industrial process timing
- Digital electronics education
- FPGA and VLSI design training

10. Advantages

- Combines two timer functions in one design.
- Helps develop practical Verilog programming skills.
- Demonstrates sequential logic and counter design.
- Supports simulation before hardware implementation.
- Can be extended with additional digital features.

12. Future Enhancements

- Audible alarm at countdown completion.
- User-configurable countdown presets.
- Lap-time recording.
- Push-button debouncing.
- Improved display interface.
- Physical FPGA board implementation.

13. Conclusion

The FPGA-Based Digital Stopwatch with Countdown Timer demonstrates the use of Verilog HDL to design and verify a digital timing system. It integrates clock division, up/down counters, control logic, and seven-segment display decoding. The project provides practical experience in RTL design, simulation, and FPGA implementation.

