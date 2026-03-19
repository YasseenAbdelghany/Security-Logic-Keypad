# Security-Logic-Keypad

## Project Report: Digital Security Keypad Using Logic Circuits

### Project Objective
The goal of this project is to design and implement a security keypad system using digital circuits. The system processes, stores, and compares digital signals, enabling a buzzer alarm or LED indicator in response to correct or incorrect secret code inputs.

---

## Components and Their Functions

### 1. Power Supply
- **Function:** Provides a stable voltage (5V) to power all electronic components.
- **Importance:** Ensures consistent operation of the ICs and other components.

### 2. 4-Digit 7-Segment Display
- **Function:** Displays user inputs, system states, or results.
- **Connection:** Connected to the decoder output to translate binary signals into readable numbers.

### 3. 5 × 4 DIP Switch
- **Function:** Provides manual binary inputs (0 or 1) used to set the secret code or reference values.
- **Connection:** Inputs are connected to Flip-Flops or decoders for storage or processing.

### 4. 3 × 4 Keypad
- **Function:** Allows the user to input the secret code and sends signals to the encoder for processing.
- **Connection:** Directly connected to the encoder.

### 5. 8 D-Flip Flop (74LS175)
- **Function:** Stores binary inputs from the keypad or DIP switch and outputs values to other components such as comparators or decoders.
- **Connection:** Outputs (Q0–Q7) are linked to the comparator inputs.

### 6. 4 Comparators (74LS85)
- **Function:** Compare the user-inputted values with the stored reference code and determine whether the input matches the secret code.
- **Connection:** A inputs are from stored values, and B inputs are from keypad entries.

### 7. NOT Gate (74LS04)
- **Function:** Inverts binary signals (1 → 0 or 0 → 1).
- **Use:** Used to adjust or correct signal states within the circuit.

### 8. Decoder
- **Function:** Converts binary data into a format suitable for display (e.g., for the 7-segment display).
- **Use:** Displays input or system status.

### 9. Demultiplexer
- **Function:** Routes a single input signal to one of several outputs based on control signals.
- **Use:** Used to distribute signals to components like the display or buzzer.

### 10. Timer 555
- **Function:** Generates clock pulses to synchronize operations.
- **Use:** Can also define the buzzer alarm duration.

### 11. Capacitors (2 × 10nF) and Resistors (2 × 1000kΩ)
- **Capacitors:** Smooth electrical signals or generate clock pulses.
- **Resistors:** Used in pull-up circuits or for timing in the 555 timer.

### 12. Encoder
- **Function:** Converts keypad inputs into binary signals.
- **Use:** Facilitates signal processing within the system.

### 13. Logic Gates (AND, OR, NOR)
- **AND Gate:** Activates output when all inputs are high (1).
- **OR Gate:** Activates output when any input is high (1).
- **NOR Gate:** Outputs a high signal only if all inputs are low (0).

### 14. JK Flip-Flop (74LS38)
- **Function:** Stores and manipulates binary signals.
- **Use:** Used for synchronous operations in the circuit.

### 15. Bit Counter
- **Function:** Counts signals or steps executed.
- **Use:** Helps in limiting the number of input attempts for the secret code.

### 16. Buzzer Alarm
- **Function:** Emits an audible alert when an incorrect code is entered or when the input limit is exceeded.
- **Connection:** Connected to the logic gate outputs to indicate error conditions.

### 17. LEDs (2 × LED)
- **Function:** Indicates system status (e.g., success or failure).
- **Use:** Turns on based on comparator output results.

---

## How the Project Works
1. **Input:** The user enters a code through the keypad or DIP switches.
2. **Storage:** Inputs are stored in Flip-Flops (e.g., 74LS175 or 74LS38).
3. **Processing and Comparison:** The entered code is compared to a pre-stored reference code using comparators (74LS85).
4. **Result:**
   - If the codes match, the system triggers an LED to indicate success.
   - If the codes do not match, a buzzer alarm is activated.
5. **Reset:** The system can be reset through an external control to allow new input.

---

## Applications
1. Digital security systems.
2. Code-based locking mechanisms.
3. Industrial control systems.

---

## Conclusion
This project demonstrates the practical application of digital logic circuits in creating a secure keypad system. It highlights how components like Flip-Flops, comparators, encoders, and logic gates work together to process and verify user inputs. The system is modular and can be extended to include additional features like more input attempts, advanced displays, or integration with microcontrollers.

---

## Made by
- Yasseen Ahmed (23101608)
- Ahmed Khaled (23101545)
- Mostafa Mohamed (23101601)
- Youssef Ramadan (23101614)