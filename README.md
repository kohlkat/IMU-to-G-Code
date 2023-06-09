# 🤖 IMU-to-G-code Real-time Conversion System

This project aims to create a system that can convert IMU (Inertial Measurement Unit) data into G-code for CNC machines, while also considering safety precautions to prevent damage to the CNC machine and the workpiece. The system uses a microcontroller with an RTOS (Real-Time Operating System) for efficient multitasking and processing.

## 📚 Table of Contents
1. [🔩 Hardware Requirements](#hardware-requirements)
2. [💾 Software Requirements](#software-requirements)
3. [🛠️ Setup and Configuration](#setup-and-configuration)
4. [📟 Microcontroller Code Structure](#microcontroller-code-structure)
5. [🔰 Safety Precautions and Collision Detection](#safety-precautions-and-collision-detection)
6. [👓 Augmented Reality Capabilities](#augmented-reality-capabilities)
7. [🚀 Future Development](#future-development)
8. [🎯 Goals](#goals)
9. [🌟 Getting Started](#getting-started)
10. [💡 Contributing](#contrubuting)
11. [📄 License](#license)
12. [📬 Contact](#contact)

## 🔩 Hardware Requirements
- Inertial Measurement Unit (IMU): 3DM-CX5-25
- Microcontroller: STM32F7 series
- CNC machine

## 💾 Software Requirements
- Real-Time Operating System (RTOS): FreeRTOS
- Microcontroller Libraries: MSCL (MicroStrain Communication Library)
- G-code generation library

## 🛠️ Setup and Configuration
1. Set up the microcontroller with the chosen RTOS (FreeRTOS).
2. Configure the IMU with the MSCL library.
3. Implement the G-code generation logic.

## 📟 Microcontroller Code Structure
1. Initialize system
   - Configure microcontroller and peripherals
   - Initialize FreeRTOS
2. Start tasks
   - IMU data acquisition task
   - G-code generation task
   - G-code sending task
3. Run tasks in parallel (see [Microcontroller Flowchart](#microcontroller-flowchart) for detailed steps)

## 🔰 Safety Precautions and Collision Detection
The system checks for potential collisions by analyzing the generated G-code and comparing it with the current state of the CNC machine and workpiece. If a potential collision is detected, the system injects precautionary G-code to prevent damage.

## 👓 Augmented Reality Capabilities
The project aims to include AR capabilities, allowing users to visualize the CNC process in real-time with additional overlays and information.

## 🚀 Future Development
Potential future development includes gesture control, user-guided machining, and a wide range of applications across various industries.

### 🎯 Goals
✅ Choose a suitable microcontroller \
✅ Choose an RTOS \
✅ Set up communication with the IMU \
✅ Convert IMU data to G-code \
✅ Implement safety precautions \
✅ Send G-code to the CNC machine \
🔄 Implement augmented reality capabilities \
🔄 Gesture control \
🔄 Further user base research and development

## 🌟 Getting Started

1. Familiarize yourself with the chosen IMU and platform for the prototype phase.
2. Set up a development environment and clone this repository.
3. Review the existing code and documentation to understand the current state of the project.
4. Explore the open issues and feature requests to identify areas where you can contribute.
5. Reach out to the project maintainers for guidance or to propose new ideas.

## 💡 Contributing

We welcome contributions from the community! Please follow these steps to contribute to the project:

1. Fork this repository.
2. Create a branch with a descriptive name, such as `feature/imu-data-acquisition` or `bugfix/motion-control`.
3. Commit your changes to the branch, following the [commit message guidelines](https://chris.beams.io/posts/git-commit/).
4. Push your changes to your fork.
5. Open a pull request against the main repository, providing a clear description of your changes and any relevant context.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 📬 Contact

For questions, suggestions, or support, please reach out to the project maintainers at [dkohlkat@gmail.com](mailto: dkohlkat@gmail.com).

