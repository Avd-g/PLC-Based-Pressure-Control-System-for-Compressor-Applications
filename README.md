# PLC-Based-Pressure-Control-System-for-Compressor-Applications
### PLC-Based Pressure Control System for Compressor Applications

This repository contains a comprehensive implementation of a programmable logic controller (PLC) program designed to maintain and control pressure within a compressor receiver system. The logic ensures automated management of compressor activation based on real-time pressure monitoring using two distinct pressure switches and provides visual feedback via an indicator light.

#### Project Overview:

* **Objective:** Automatically maintain receiver pressure between defined limits (90 psi and 110 psi) using PLC logic, ensuring efficient compressor operation and system safety.
* **Components:** PLC with clearly defined input/output (I/O) points, including two pressure switches, a compressor pump, and a visual indicator.

#### Implementation and Key Features:

* **Pressure Switch Logic:**

  * **Low Pressure Switch:** Activates at 90 psi to indicate sufficient pressure for system operations.
  * **High Pressure Switch:** Activates at 110 psi to signal maximum allowable pressure.

* **Actuation and Feedback:**

  * **Compressor Pump Control:** Automatically starts and stops based on the logic states of the low and high pressure switches.
  * **Indicator Light:** Illuminates when system pressure is above the low-pressure threshold (90 psi), providing immediate visual status indication.

* **PLC I/O Assignment:**

  * **Inputs:**

    * I:0/0: Low-pressure switch (activates ≥ 90 psi).
    * I:0/1: High-pressure switch (activates ≥ 110 psi).
  * **Outputs:**

    * O:0/0: Compressor pump control.
    * O:0/1: Pressure status indicator light.

#### Test Criteria and Performance Evaluation:

* Conducted detailed testing and validation to ensure:

  * Immediate pump activation at system startup.
  * Indicator light responsiveness to changes in system pressure.
  * Automatic compressor deactivation upon reaching high-pressure threshold.
  * Consistent behavior across varying switch conditions and pressure states.

#### Strengths and Learning Points:

* **Robust PLC Logic:** Reliable and maintainable control logic suitable for real-world compressor applications.
* **Clear Operational Feedback:** Immediate visual status via an indicator enhances operational safety and system monitoring.
* **Educational Insights:** Emphasizes practical troubleshooting, iterative testing, and reinforces best practices in real-world PLC programming scenarios.

#### Future Development:

* Integration of advanced pressure sensing and data logging for enhanced monitoring.
* Implementation of safety interlocks and additional alarms for broader industrial applications.

This project effectively demonstrates fundamental PLC programming techniques, providing a robust platform for further development and practical application in industrial control scenarios.
