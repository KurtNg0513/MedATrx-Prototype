# MedATrx: Automated Networked Medicine Dispenser


## 📌 System Overview
MedATrx is a hardware-software prototype designed specifically to assist individuals with ADHD by addressing executive dysfunction and ensuring consistent medication routines. Built within a Raspberry Pi environment, the system bridges physical hardware controls with networked software monitoring to ensure operational stability, secure data sharing, and environmental tracking.

## ⚙️ Architecture & Technical Stack
* **Core Environment:** Raspberry Pi
* **Software Architecture:** Programmed in Python, leveraging PyQt5 for the on-device touchscreen GUI and a Flask web server for the remote IoT dashboard.
* **Hardware Integration:** 
  * Stepper motor configured for precise 22.5-degree rotations to drive a 14-slot medication tray (with 2 dedicated refill reminder slots).
  * Temperature and humidity sensor integrated to monitor the environment and prevent medication degradation.
  * 16-key keypad for on-device settings and manual control.
* **Monitoring & Diagnostics:** Custom visual event logging system utilizing an AI camera to securely capture and store user photos upon dispensing.

## 🔐 Key Engineering & Security Contributions
* **Secure Dispensing & Verification:** Triggers the AI camera to capture a photo of the user upon dispensing, storing the image in a local activity log for caregiver review.
* **Anti-Tamper Lockout:** Implements a 30-second system lock-out and an orange LED warning if the dispense button is pressed outside the designated alarm window.
* **Hyperfocus Interruption:** Utilizes a high-pitched active buzzer and a flashing RGB LED to successfully interrupt hyperfocus and alert the user.
* **Refill Enforcement:** Enforces a mechanical stop upon reaching the refill slots, requiring manual user confirmation on the touchscreen before resuming rotation.

## 🏆 Exhibitions & Recognition
* **OACETT "From Grid to Greatness" 2026 Tradeshow:** Successfully pitched the MedATrx prototype to senior leadership, earning an exclusive invitation from Director of Professional Affairs David Terlizzi to showcase the system as a product exhibitor.
