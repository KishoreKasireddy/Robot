
# Bluetooth Controlled Servo Robot

This project demonstrates controlling servos using voice commands received via a Bluetooth module (HC-05). The Arduino receives voice commands through the Bluetooth module and moves the servos accordingly.

## Components Used

- Arduino
- HC-05 Bluetooth Module
- Servo Motors (6 in total)
- Jumper Wires
- Breadboard

## Circuit Connections

1. Connect the HC-05 module to the Arduino:
   - HC-05 RX to Arduino pin 0 (via voltage divider to 3.3V)
   - HC-05 TX to Arduino pin 1
   - HC-05 VCC to 5V
   - HC-05 GND to GND

2. Connect the servo motors to the Arduino:
   - Head servo to pin 13
   - Right hand servos to pins 9, 10, and 11
   - Left hand servos to pins 5, 6, and 7

## Usage

1. Upload the provided code to your Arduino.
2. Pair the HC-05 module with your mobile phone. The default pairing password is usually `1234` or `0000`.
3. Open a serial Bluetooth terminal app on your mobile phone and connect to the HC-05 module.
4. Send the following commands to control the servos:
   - `hello`: The robot waves its right hand.
   - `shake hand`: The robot performs a handshake motion.
   - `hands up`: The robot raises both hands.
   - `hands down`: The robot lowers both hands.

## Code Explanation

The code initializes the Bluetooth module and the servo motors in the `setup` function. It continuously checks for incoming data from the Bluetooth module in the `loop` function. Based on the received command, it calls the corresponding function to move the servos.

The servo movements are defined in the following functions:
- `say_hi()`: Moves the right hand in a waving motion.
- `hands_up()`: Raises both hands.
- `hands_down()`: Lowers both hands.
- `shake_hand()`: Moves the right hand in a handshake motion.


## Acknowledgements

- This project uses the [Arduino](https://www.arduino.cc/) platform.
- The [HC-05 Bluetooth Module](https://www.electronicwings.com/nodemcu/hc-05-bluetooth-module-interfacing-with-arduino-uno) is used for Bluetooth communication.

Mechanical Desigining , Dimensions and Layouts are hidden.
For full information  Contact- kishorekasireddi4@gmail.com 
