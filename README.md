# Pololu Robot Navigation and Control

This repository contains my solutions for controlling and navigating the Pololu 3pi+ 2040 robot using Lingua Franca. The project involves utilizing sensors, motors, and reactive programming techniques to achieve various tasks.

## Solutions Overview

### 1. **Robot Drive Solution**
- Implemented the `Motors` reactor to control motor power.
- The robot moves forward in the `DRIVING` mode and stops in the `STOPPED` mode.
- Verified motor control functionality using PWM signals.

### 2. **Encoder Distance Conversion**
- Developed a reactor `AngleToDistance` to convert encoder readings (degrees) into distance traveled (meters).
- Calculated and displayed the distance traveled by each wheel using the encoder data.
- Ensured accurate conversion and functionality in the `RobotEncoderSolution.lf`.

### 3. **Square Navigation with Gyroscope**
- Created a modal Lingua Franca program, `RobotSquareSolution.lf`, to navigate the robot in a square pattern.
- Utilized the `GyroAngle` reactor to compute the robot's angle and ensure accurate 90-degree turns.
- Configured the robot to drive 0.5 meters forward before each turn.

### 4. **Obstacle Avoidance**
- Enhanced the square navigation program with obstacle avoidance.
- Integrated the `Bump` reactor to detect obstacles and modify the robot's path dynamically.
- Ensured the robot could back off and avoid collisions while navigating.

## Key Features
- Reactive programming with Lingua Franca.
- Integration of multiple sensors (gyroscope, encoders, bump sensors).
- Modal programs for behavior-based robot control.
- Accurate distance estimation and real-time obstacle avoidance.

## Technologies Used
- **Lingua Franca** for reactive programming.
- Pololu 3pi+ 2040 robot with sensors and motor drivers.
- Gyroscope, encoders, and bump sensors for navigation and control.

Feel free to explore the individual `.lf` files for detailed implementations!
