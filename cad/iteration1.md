# Iteration 1 – Expanding Beyond the Original Chassis

<div align="center">

## Overall CAD Design

<img src="pictures/iteration1_autodesk.png" alt="Iteration 1 CAD" width="800"/>

<br><br>

## Drivetrain Layout

<img src="pictures/iteration1_drivetrain_autodesk.png" alt="Drivetrain Layout" width="800"/>

<br><br>

## Structural Issue Encountered

<img src="pictures/WD_problem_irl.png" alt="PLA Chassis Bending" width="500"/>

</div>

---

## Objective

The original rover chassis from the robotics kit was designed for significantly smaller motors and fewer onboard sensors. After upgrading the drivetrain with larger motors, LiDAR, ultrasonic sensors, a camera, Raspberry Pi, motor drivers, and additional electronics, the original chassis no longer had sufficient space.

Since I did not have access to a CNC machine, the chassis had to be redesigned as a 3D-printable assembly using PLA. The goal of this iteration was to create a larger platform while remaining within the build volume of my desktop 3D printer.

---

## Design Decisions

- Increased chassis footprint to accommodate larger motors.
- Added multiple levels for electronics and sensors.
- Created dedicated mounting locations for:
  - Raspberry Pi
  - Motor drivers
  - LiDAR
  - Ultrasonic sensors
  - Camera
- Used aluminum standoffs to separate the electronics layers.
- Designed the base plate to fit within the maximum printable area of the printer.

---

## What Worked

- Every component fit within the available space.
- Sensor placement provided good fields of view.
- Electronics were easy to access and organize.
- The modular stacked design made future modifications straightforward.

---

## Problems Discovered

Although the packaging was successful, this design revealed an important mechanical issue.

### Weight Distribution

The four DC gear motors were the heaviest components on the rover and were mounted near the outer edges of the chassis.

The large PLA base plate was primarily supported around its perimeter, leaving a long unsupported span through the middle. As additional electronics were installed, the chassis began to flex noticeably.

### Structural Rigidity

Because the chassis was printed from PLA and lacked reinforcing ribs or structural supports, the base plate bent significantly under load.

Rather than risking damage to the printed chassis, I decided to redesign the mechanical structure before continuing development.

---

## Lessons Learned

- Designing for available space is only part of the engineering process.
- Structural stiffness is just as important as packaging.
- Future iterations will prioritize improved weight distribution, increased rigidity, and better support for the drivetrain.
