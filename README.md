# 🔐 Password & Fingerprint Based Door Locking System

## Embedded Systems Project | Electronics & Communication Engineering

A prototype **electronic door locking and access-control system** developed using a microcontroller, keypad-based password authentication, fingerprint verification, and a 16×2 LCD display.

The project demonstrates how embedded hardware and software can be combined to create a secure electronic access-control system. The user can interact with the system through a keypad and fingerprint interface, while the LCD provides real-time instructions and authentication status.

---

# 📌 1. Project Overview

Traditional door-locking systems generally depend on physical keys. This project was developed to demonstrate an electronic alternative using **password and fingerprint-based authentication**.

The system combines:

- Password-based authentication
- Fingerprint-based authentication
- 4×4 matrix keypad
- 16×2 LCD display
- Microcontroller-based control
- Electronic lock-control logic
- Embedded programming
- Hardware prototyping and testing

The main purpose of the project is to verify the user's credentials before allowing access to the protected door.

---

# 🎯 2. Project Objectives

The main objectives of this project are:

- To develop an electronic door-locking system.
- To implement password-based user authentication.
- To integrate fingerprint-based authentication.
- To interface a keypad with a microcontroller.
- To interface a 16×2 LCD for user interaction.
- To display authentication instructions and system status.
- To control the door-locking mechanism after successful authentication.
- To demonstrate practical embedded-system hardware integration.
- To develop and test a working security-oriented prototype.

---

# 🧩 3. Main Features

### 🔑 Password Authentication
The user can enter a password using the keypad.

### 👆 Fingerprint Authentication
The system provides a fingerprint-based authentication interface.

### 🖥️ LCD User Interface
A 16×2 LCD displays system prompts and authentication messages.

### 🔒 Electronic Access Control
Access is controlled according to the authentication result.

### 🔧 Embedded Hardware
The project integrates multiple electronic modules into a single prototype.

### 💻 Software + Hardware Integration
The system was programmed and tested through an Arduino-based development environment.

---

# 📸 4. Actual Project Hardware

The following photographs show the **actual hardware and development setup** used during the project.

## Password Entry and Hardware Setup

![Door Locking System - Password Entry](images/door-locking-system-1.jpg)

The photograph shows the microcontroller development setup, keypad, 16×2 LCD, wiring, and computer-based programming environment used during project development.

# 🏗️ 5. System Architecture

```text
                    +----------------------+
                    |        USER          |
                    +----------+-----------+
                               |
              +----------------+----------------+
              |                                 |
              v                                 v
      +---------------+                 +---------------+
      |    Keypad     |                 |  Fingerprint |
      | Password Input|                 |    Sensor     |
      +-------+-------+                 +-------+-------+
              |                                 |
              +---------------+-----------------+
                              |
                              v
                    +--------------------+
                    |   Microcontroller  |
                    |  Authentication    |
                    |      Logic         |
                    +---------+----------+
                              |
              +---------------+---------------+
              |                               |
              v                               v
      +---------------+                +---------------+
      |    16×2 LCD   |                | Lock Control  |
      | User Feedback |                |   Mechanism   |
      +---------------+                +-------+-------+
                                                  |
                                                  v
                                           +-------------+
                                           | Door Access |
                                           +-------------+
```
# 🔄 6. Working Principle
```
The system follows an authentication-based access-control process.
START
  |
  v
Initialize Hardware
  |
  v
Display Authentication Prompt
  |
  +--------------------------+
  |                          |
  v                          v
Password Input          Fingerprint Input
  |                          |
  +------------+-------------+
               |
               v
      Authentication Check
               |
          +----+----+
          |         |
          v         v
        VALID     INVALID
          |         |
          v         v
    Allow Access   Retry
          |
          v
    Lock Control
          |
          v
         END
```
he microcontroller receives the user's authentication input, processes it, updates the LCD, and controls the access-control output according to the authentication result.
# 🔑 7. Password Authentication

The keypad is used to enter the user's password.

Typical sequence:
```
System Ready
     |
     v
Enter Password
     |
     v
Keypad Input
     |
     v
Password Verification
     |
   +---+---+
   |       |
 Valid   Invalid
   |       |
   v       v
Access    Retry
```
The keypad therefore acts as the primary user-input interface for password-based authentication.
# 🖥️ 8. 16×2 LCD Display

A 16×2 character LCD is used as the local user interface.

The LCD can provide:

- Password-entry instructions
- Fingerprint prompts
- Authentication information
- System status
- Retry messages
- Access-related messages

The LCD makes the system easier to operate by providing direct visual feedback to the user.
# 🔢 9. Keypad Interface

A matrix keypad is used to provide user input.

The keypad can be used for:

- Password entry
- User interaction
- Authentication control
- Selecting input options

The keypad is connected to the microcontroller and processed through the embedded program.
# 🔒 10. Door Lock Control

After successful authentication, the controller generates the required control signal for the door-locking mechanism.

The basic concept is:
```
Authentication
      |
      v
Microcontroller
      |
      v
Lock Control
      |
      v
Door Access
```
# 🧪 11. Development and Testing Setup

The project was developed and tested using a computer-based embedded programming environment.

The development process involved:
```
Write Program
     |
     v
Compile
     |
     v
Upload to Controller
     |
     v
Connect Hardware
     |
     v
Test Input / Display / Authentication
     |
     v
Debug
     |
     v
System Validation
```
# 🔌 12. Hardware Integration

The major hardware sections are integrated as follows:
```
                 +----------------+
                 |    Keypad      |
                 +--------+-------+
                          |
                          v
                 +----------------+
                 |                |
                 | Microcontroller|
                 |                |
                 +--------+-------+
                          |
             +------------+------------+
             |                         |
             v                         v
      +-------------+           +-------------+
      |    LCD      |           | Fingerprint |
      |   16×2      |           | Interface   |
      +-------------+           +-------------+
                          |
                          v
                  +-------------+
                  | Lock Control|
                  +-------------+
```
# 🚀 13. Future Improvements

Possible future improvements include:

- Multiple fingerprint-user support
- Password change functionality
- Failed-attempt lockout
- Alarm after repeated invalid attempts
- Secure credential storage
- Access-event logging
- Real-time clock integration
- Mobile monitoring
- IoT-based access monitoring
- Dedicated PCB development
- Enclosed mechanical lock assembly
- Tamper detection
# 📂 14. Repository Structure
```
door-locking-system/
│
├── README.md
│
├── PROJECT_INFO.md
│
├── images/
│   ├── door-locking-system-1.jpg
│   └── door-locking-system-2.jpg
│
├── src/
│   └── [your actual source code]
│
├── circuit/
│   └── [circuit diagram if available]
│
└── docs/
    └── [supporting documentation]
```

# 👨‍💻 15. Author
Vattam Madhu Kumar

Electronics & Communication Engineering

Velagapudi Ramakrishna Siddhartha Engineering College
Vijayawada, Andhra Pradesh, India

GitHub

https://github.com/MadhuKumar-003

LinkedIn

https://linkedin.com/in/madhu-kumar-vattam/
