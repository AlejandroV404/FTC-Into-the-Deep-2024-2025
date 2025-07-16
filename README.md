# FTC Robotics Control System – 2024–2025
https://theorangealliance.org/teams/12397

This repository contains the complete control system I developed for our FTC robotics team during the 2024–25 season. It includes autonomous and tele-op code written in Java, built on the FTC SDK.

> ⚠️ **Note:** Due to a Git misconfiguration during the season, many commits were incorrectly attributed to a teammate so I reuploaded it. This code reflects my original work and programming contributions.


## 🧠 Features
- **Autonomous Pathing**: Odometry-based navigation with encoder feedback
- **RoadRunner Autonomous**: For precise movement and rotation
- **Multi-threading**: Input handling and subsystem control during TeleOp
- **Modular Architecture**: Easy to extend and debug
- **Failsafes**: Safety checks for motor protection and sensor validation

## 🔧 Technologies Used
- Java (FTC SDK)
- OnBot Java & Android Studio
- REV Expansion Hub & IMU
- goBILDA Encoders
- LinearOpMode & OpMode implementations

## 📁 Code Structure
├── Autonomous/
│ AutoByRRSpecimen.java
│ AutoByRRBucket.java
│ [Other tests and versions included to show progress]
├── TeleOp/
│ RobotCentricSolo.java
│ RobotCentricDuo.java
├ Utils/
│ RobotHardware.Java
│ MeepMeepTesting
│ Tuning


## 🧪 How to Use
1. Clone or download the repository
2. Import into Android Studio or upload via OnBot Java
3. Configure hardware map to match your team's robot
4. Select your OpMode on the Driver Station and test
   [for RoadRunner Usage you will first need to tune your robot for roadrunner. Here's a guide: learnroadrunner.com]

## 🏆 About the Project
This code was used to:
- Qualify for FTC State Championships
- Win the **Control Award** at regional competition
- Showcase advanced motion algorithms and autonomous design

## ✍️ Author's Note

This was my first year programming for FTC robotics. I taught myself Java and learned the FTC SDK and control algorithms as the season progressed. I also served as the sole mechanical builder and programmer for our robot, taking full responsibility for hardware, software, and Operational development.

It was a challenging but incredibly rewarding experience. I’m proud of what I accomplished independently, and I hope this code can help or inspire other students pursuing robotics with limited resources or experience.

## 🧩 Extra Notes (Technical Considerations)

> _FTC SDK-specific notes and formatting guidelines (from BlocksOpModeCompanion and ExportToBlocks usage):_

- Classes must be in the `org.firstinspires.ftc.teamcode` package.
- For easy access to `opMode`, `hardwareMap`, `telemetry`, `gamepad1`, and `gamepad2`, classes can extend `BlocksOpModeCompanion`.
- Public static methods can be annotated with `@ExportToBlocks` and must use supported parameter types (e.g., `OpMode`, `HardwareMap`, `boolean`, `int`, `double`, `String`, etc.).
- Specific UI improvements were made:
  - Changed "Save completed successfully." text color for better visibility on green background.
  - Fixed the "Download image" feature to work with text blocks present in the OpMode.
