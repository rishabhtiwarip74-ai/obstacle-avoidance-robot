\# Obstacle Avoidance Robot 🤖



\## Overview

This project is an autonomous robotic vehicle designed to navigate environments without human intervention. By utilizing ultrasonic sensors, the robot continuously scans its path for physical barriers. When an obstacle is detected within a predefined threshold, the system processes this data in real-time to alter the robot's trajectory, ensuring collision-free movement.



\## Features

\* \*\*Autonomous Navigation:\*\* Moves independently without requiring remote control.

\* \*\*Real-Time Detection:\*\* Uses ultrasonic sound waves to calculate exact distances to approaching objects.

\* \*\*Dynamic Pathfinding:\*\* Automatically reverses and pivots when a blocked path is encountered.



\## Hardware Components

\* Microcontroller (e.g., Arduino Uno / ESP32)

\* Ultrasonic Sensor (HC-SR04)

\* Motor Driver Module (e.g., L298N)

\* 2x or 4x DC Motors \& Wheels

\* Robot Chassis

\* Power Supply / Battery Pack

\* Jumper Wires



\## Software \& Tools

\* \*\*Language:\*\* Embedded C / C++

\* \*\*Environment:\*\* Arduino IDE



\## How It Works

1\. The robot moves forward by default, driving all DC motors simultaneously.

2\. The front-mounted ultrasonic sensor continuously emits high-frequency sound waves and listens for their echo to calculate the distance to the nearest object.

3\. The microcontroller evaluates this distance data in a continuous loop.

4\. If the distance falls below the safe threshold (e.g., 15 cm), the microcontroller signals the motor driver to stop the motors immediately.

5\. The robot then executes an avoidance maneuver: reversing slightly, turning left or right to find a clear path, and resuming its forward motion.

