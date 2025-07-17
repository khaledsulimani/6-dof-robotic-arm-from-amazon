# 🤖 6-DOF Robotic Arm with 6 Servo Motors

This project is a 6-DOF (Degrees of Freedom) robotic arm built with a robotic clamp claw. The arm can rotate up to 180 degrees and is designed for STEM educational purposes, ideal for teaching robotics, automation, and programming. 🛠📚

## 🔧 Project Overview

The robot is equipped with 6 servo motors, each controlling one degree of freedom, allowing for high flexibility and precision. The arm is designed to simulate industrial robot parts, making it an excellent tool for learning about robotics in various fields, including engineering, computer science, and automation.

## 💡 Design Process

The design of the robotic arm was made using two main software tools:
1. *TinkerCAD* 🖥: Used for designing basic parts and joints, allowing for quick prototyping.
2. *Blender* 🎨: Used for more detailed and complex parts like the gripper and claws, providing high-quality 3D models for 3D printing.

## 📂 Files

- *STL Files*: Below are the STL files for the robotic arm parts. These can be printed using a 3D printer.
  - [Servo base.stl](./files/Servo_base.stl)
  - [Servo MG996R.stl](./files/Servo_MG996R.stl)
  - [Brackets.stl](./files/Brackets.stl)
  - [Claw.stl](./files/Claw.stl)
  - [U-shaped mount brackets.stl](./files/U_shaped_mount_brackets.stl)
  - [Base.stl](./files/Base.stl)

## 🛠 Instructions for Assembly

1. *Print the Parts*: Use a 3D printer to print the STL files. Ensure to use durable plastic like PLA or ABS for best results.
2. *Assemble the Arm*: Begin by attaching the parts in the following order: Base, U-shaped Mount Brackets, Servo Base, Brackets, Servo MG996R, Claw.
3. *Servo Motor Installation*: Connect each servo motor to the corresponding joint on the arm (6 in total). Ensure to properly align the servos for accurate movement.
4. *Wiring and Electronics*: Connect the motors to a microcontroller (e.g., Arduino or Raspberry Pi) to control the servos. Ensure you have the proper power supply and motor drivers.
5. *Programming*: Upload the control code to your microcontroller to begin controlling the robotic arm. You can use any suitable library, such as Servo.h in Arduino, to manage the servo movements.

## 📸 Project Results

### *the last form for robotic arm*:![صورة واتساب بتاريخ 1447-01-22 في 04 21 54_85767a8d](https://github.com/user-attachments/assets/003248e5-052c-4b8f-92d7-aba742702f45)

## 💻 Control and Programming

To control the robot arm, you'll need to write code to control each of the 6 servo motors. Here's a simple example in Arduino:

```cpp
#include <Servo.h>

Servo servo1, servo2, servo3, servo4, servo5, servo6;

void setup() {
  servo1.attach(9);  // Attach each servo to a PWM pin
  servo2.attach(10);
  servo3.attach(11);
  servo4.attach(12);
  servo5.attach(13);
  servo6.attach(14);
}

void loop() {
  servo1.write(90);  // Set servo positions
  servo2.write(90);
  servo3.write(90);
  servo4.write(90);
  servo5.write(90);
  servo6.write(90);
  delay(1000);  // Wait for 1 second
}
```
## 🧑‍💻 Author

- **khaled mahmoud sulaimani** – [@khaledsulimani](https://github.com/khaledsulimani)
