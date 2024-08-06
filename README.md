# DC Motor Control with Arduino and L298N Motor Driver

## Overview

This project demonstrates how to control two DC motors using an Arduino and the L298N motor driver. The motors are controlled to rotate in both clockwise and counterclockwise directions. The code also includes optional PWM (Pulse Width Modulation) for speed control.

## Components Used

- **Arduino Board**: UNO or any compatible board
- **L298N Motor Driver**: For controlling motor direction and speed
- **DC Motors**: Two motors
- **Jumper Wires**: To connect the Arduino and L298N
- **Power Supply**: 9V battery or similar
- **Breadboard** (optional): For wiring connections

## Wiring Instructions

### 1. L298N Motor Driver Pinout Diagram
Refer to the L298N pinout diagram for detailed pin connections: 
![L298N Pinout Diagram](https://github.com/shathalshehri/DCMotorControl/blob/main/Image%201.jpg)

### 2. Connect Your Motors with L298N Motor Driver
Connect your DC motors to the L298N motor driver as shown in the image: 
![Motor Connections](https://github.com/shathalshehri/DCMotorControl/blob/main/Image%203.jpg)

### 3. Connect Your L298N Pins with Arduino UNO Pins
Follow this diagram to connect the L298N pins to the Arduino UNO pins: 
![Arduino to L298N Connections](https://github.com/shathalshehri/DCMotorControl/blob/main/Image%202.jpg)

### 4. Controlling Speed
If you want to control the speed of the motors, you will need to connect PWM pins and configure them in the code. Check out this image for the extra setup needed: 
![Speed Control Setup](https://github.com/shathalshehri/DCMotorControl/blob/main/Image.jpg)

### 5. Real-Life Setup
See the final setup with all connections, wires, and the Arduino in action: 
![Real-Life Setup](https://github.com/shathalshehri/DCMotorControl/blob/main/4.jpg)

## Demo

Watch the demo of the DC motor control in action: 
![Demo](https://github.com/shathalshehri/DCMotorControl/blob/main/demo.gif)

## Arduino Code

To see the full code for controlling the DC motors using the L298N motor driver, check out the [DC_motor_with_H_bridge0.ino](https://github.com/shathalshehri/DCMotorControl/blob/main/DC_motor_with_H_bridge0.ino) file in the repository.

## How It Works

1. **Setup**: Initializes the pins for controlling the motors and optionally sets PWM pins for speed control.
2. **Loop**:
   - **Clockwise Rotation**: Sets the direction pins to rotate both motors clockwise for 3 seconds.
   - **Pause**: Stops the motors for 1 second.
   - **Counterclockwise Rotation**: Changes direction to rotate both motors counterclockwise for 3 seconds.
   - **Pause**: Stops the motors for 1 second before repeating the cycle.

## Optional Features

- **Speed Control**: Adjust the `analogWrite` values for PWM pins to control the speed of the motors. `0` is off and `255` is the maximum speed.

## Troubleshooting

- **Motors Not Running**: Check all connections and ensure that the power supply is properly connected.
- **Uneven Speed**: Verify the PWM values and ensure the motors are connected properly.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

Special thanks to the open-source community and Arduino documentation for their support and resources.

---

Feel free to customize this README to fit any additional details or specific instructions related to your project.
