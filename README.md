# Traffic-Light-Controller-Using-MOD-N-Counter
CAPSTONE PROJECT DESIGN DOCUMENT
Traffic-Light Controller Using MOD-N Counter
1. Project Title

Design and Implementation of a Traffic-Light Controller Using a MOD-N Counter.

2. Introduction

A traffic-light controller is a digital electronic system used to manage vehicle movement at road intersections. It controls the Red, Yellow, and Green lights in a fixed sequence to ensure safe and organized traffic flow.

This project uses a MOD-N counter and digital logic circuits to control the timing and sequence of traffic lights automatically.

3. Objectives
To design an automatic traffic-light control system.
To understand the working of MOD-N counters.
To implement sequential logic circuits.
To generate accurate timing signals.
To control traffic lights using digital electronics.
4. Components Required
IC 555 Timer
Binary counter IC (e.g., 74LS90)
Logic gates (AND, OR, NOT)
Red LED
Yellow LED
Green LED
Resistors
Capacitors
Breadboard
Connecting wires
5V DC power supply
5. Block Diagram

Clock Generator → MOD-N Counter → Decoder / Control Logic → Traffic Lights

6. Working Principle

The 555 timer generates clock pulses at regular intervals. These pulses are supplied to the MOD-N counter.

The counter counts the incoming pulses from 0 to N−1 and then resets to zero.

The decoder circuit uses the counter outputs to control the traffic lights in the required sequence.

The traffic-light sequence is:

State	Red	Yellow	Green
1	ON	OFF	OFF
2	OFF	OFF	ON
3	OFF	ON	OFF
4	ON	OFF	OFF

The sequence repeats continuously.

7. MOD-N Counter Design

A MOD-N counter counts N distinct states before returning to its initial state.

The number of flip-flops required is:

2^m ≥ N

Where:

m = Number of flip-flops
N = Required number of states

For example, a MOD-4 counter requires:

2² = 4 states

Therefore, two flip-flops are sufficient.

8. Truth Table
Q1	Q0	Traffic Light
0	0	Red
0	1	Green
1	0	Yellow
1	1	Red
9. Applications
Road intersections
Pedestrian crossings
Automatic traffic management
Smart city traffic systems
Industrial traffic control systems
10. Advantages
Reduces the need for manual traffic control.
Provides automatic operation.
Uses simple digital electronic components.
Demonstrates sequential logic and counter applications.
11. Limitations
Fixed timing sequence.
Does not detect actual traffic density.
Requires a continuous power supply.
A basic model does not include pedestrian detection.
12. Future Scope
Add vehicle sensors to detect traffic density.
Introduce pedestrian crossing control.
Implement emergency vehicle priority.
Use a microcontroller for intelligent traffic management.
Add wireless monitoring.
13. Conclusion

The traffic-light controller using a MOD-N counter demonstrates the practical application of digital electronics and sequential circuits. The system generates a predefined sequence of traffic-light signals using clock pulses, counters, and logic gates.

This project helps understand the concepts of counters, flip-flops, timing circuits, and digital control systems.
