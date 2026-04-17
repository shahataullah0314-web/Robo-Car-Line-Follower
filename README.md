# Robo-Car-Line-Follower

This repository contains an Arduino sketch for a 5-sensor line-follower robot.

## Included Files

- `RoboCarLineFollower.ino` - Main Arduino sketch implementing PID-based line following with lost-line pivot recovery.

## Features

- 5 infrared line sensors on analog pins `A0` through `A4`
- Dual H-bridge motor control with PWM on pins `9` and `10`
- PID steering with stronger outer sensor weighting for sharp turns
- Automatic pivot recovery when the line is lost

## Usage

1. Open `RoboCarLineFollower.ino` in the Arduino IDE.
2. Select the correct board and port.
3. Upload to your Arduino-compatible line follower robot.
4. Adjust `Kp`, `Kd`, and `baseSpeed` values as needed for your chassis.

## Notes

- The sketch assumes the line is darker than the background.
- Set `debugMode` to `true` to add serial debugging output if needed.
