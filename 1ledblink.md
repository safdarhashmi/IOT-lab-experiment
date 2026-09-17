# LED Blinking Experiment

## Aim
To interface a Light Emitting Diode (LED) with a microcontroller and program it to blink (turn ON and OFF) at a fixed time interval.

## Objective
- To understand the basic working of a microcontroller's digital output pins.
- To learn how to control an LED using GPIO pins.
- To write and upload a simple embedded program (using Arduino IDE / C code) that toggles the LED state at regular intervals.
- To verify the timing delay function and observe its effect on the blinking rate.

## Components Required
| Component | Quantity |
|---|---|
| Microcontroller board (e.g., Arduino Uno) | 1 |
| LED | 1 |
| Resistor (220Ω – 330Ω) | 1 |
| Breadboard | 1 |
| Jumper wires | 2–3 |
| USB cable | 1 |

## Circuit Diagram
- Connect the anode (longer leg) of the LED to a digital output pin (e.g., pin 13) through a current-limiting resistor.
- Connect the cathode (shorter leg) of the LED to GND.

## Procedure
1. Assemble the circuit on the breadboard as per the circuit diagram.
2. Connect the microcontroller board to the computer via USB.
3. Open the Arduino IDE (or relevant compiler/IDE).
4. Write the LED blinking program:

```c
int ledPin = 13;

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  digitalWrite(ledPin, HIGH);  // Turn LED ON
  delay(1000);                 // Wait 1 second
  digitalWrite(ledPin, LOW);   // Turn LED OFF
  delay(1000);                 // Wait 1 second
}
```

5. Compile and upload the program to the microcontroller.
6. Observe the LED behavior.

## Result
The LED successfully blinked ON and OFF at intervals of 1 second, confirming correct interfacing of the LED with the microcontroller's GPIO pin and successful execution of the digital output control program. The experiment demonstrates the basic principle of di
