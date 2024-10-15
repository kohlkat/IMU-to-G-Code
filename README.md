# 🤖 CNC AI-Enhanced Control System

This repository houses an innovative system designed to enhance CNC machine operations through real-time conversion of sensor data into G-code, augmented by unsupervised machine learning for optimizing performance and safety. It employs an ecosystem of hardware and software components, including IMU sensors, Raspberry Pi 4, Google Coral TPU for ML inference, and a safety-first approach. The project also integrates Lidar sensors and advanced material management capabilities.

---

## 📚 Table of Contents

- [🔩 Hardware Requirements](#-hardware-requirements)
- [💾 Software Requirements](#-software-requirements)
- [🛠️ Setup and Configuration](#-setup-and-configuration)
- [📈 System Architecture and Data Flow](#-system-architecture-and-data-flow)
- [📈 Unsupervised Machine Learning Model](#-unsupervised-machine-learning-model)
- [🔰 Safety Precautions and Collision Avoidance](#-safety-precautions-and-collision-avoidance)
- [🔄 Material Management and Selection](#-material-management-and-selection)
- [🔧 Sensor and Simulation Integration](#-sensor-and-simulation-integration)
- [🚀 Future Development](#-future-development)
- [🎯 Goals](#-goals)
- [🌟 Getting Started](#-getting-started)
- [💡 Contributing](#-contributing)
- [📄 License](#-license)
- [📬 Contact](#-contact)

---

## 🔩 Hardware Requirements

- Inertial Measurement Unit (IMU): 3DM-MX5 or similar high-precision models
- Raspberry Pi 4
- Google Coral TPU for machine learning inference
- CNC machine compatible with LinuxCNC or similar controllers
- Lidar sensors (Velodyne VLP-16 or Kinect for budget setups)
- Additional sensor options: accelerometers, gyroscopes

---

## 💾 Software Requirements

- TensorFlow Lite for ML model deployment on the Coral TPU
- LinuxCNC for CNC machine control and integration
- Python libraries: NumPy, SciPy, Matplotlib, serial, tflite-runtime
- Custom software for real-time data processing and ML inference
- OpenGL for 3D simulations with support for future VR/AR integration
- Isaac Sim for AI robotics simulation and virtual testing

---

## 🛠️ Setup and Configuration

1. **Raspberry Pi Setup**:
   - Install Linux, configure the Raspberry Pi, and install necessary drivers for Coral TPU.
2. **Coral TPU and TensorFlow Lite**:
   - Set up TensorFlow Lite on Coral TPU and deploy the pre-trained unsupervised learning model.
3. **IMU and Lidar Sensors**:
   - Connect and configure IMU sensors for real-time data collection. If using Lidar, place sensors around the CNC machine for environment scanning.
4. **LinuxCNC Setup**:
   - Install and configure LinuxCNC, ensuring compatibility with the Raspberry Pi system and CNC machine.
5. **Material Management**:
   - Ensure the material database is configured and integrated, with options for offline operation and updates via API.

---

## 📈 System Architecture and Data Flow

The architecture of the CNC AI-enhanced Control System integrates various components, including sensors, machine learning, material management, and CNC control. The system can operate both in real-time and through simulated environments for testing and training purposes.

The following components interact in the system:
- **Sensor Data Acquisition**: IMU, Lidar, and other sensors collect data in real-time.
- **Machine Learning Inference**: ML model generates optimized G-code from sensor data using Coral TPU.
- **CNC Control**: LinuxCNC executes the G-code on the machine.
- **Safety Module**: Monitors for unsafe conditions and takes action.
- **Material Management**: Material properties are considered for safety and optimization.

---

## 📈 Unsupervised Machine Learning Model

- Developed to optimize CNC operations by learning from sensor data and material properties.
- Focuses on real-time adaptation, performance optimization, and collision avoidance.
- Continuously improves through unsupervised learning from new data, including varying workpiece and tool sizes.

---

## 🔰 Safety Precautions and Collision Avoidance

- Machine learning algorithms predict and prevent collisions in real-time using sensor data and simulation.
- Integrates Lidar sensors for spatial awareness, ensuring safe machine operation.
- Dynamically adjusts operations based on conditions such as spindle speed, tool position, and material properties.

---

## 🔄 Material Management and Selection

- The system supports material selection via multiple interfaces (AR, VR, regular screen).
- A local cache of material properties is used for efficiency, and updates are fetched from an external API when connected to the internet.
- Materials are selected based on parameters like hardness, tensile strength, and thermal conductivity, which influence tool paths and speeds.
- Integrated into the safety and machine learning components to ensure safe and optimized machining.

---

## 🔧 Sensor and Simulation Integration

- **Lidar Integration**: Multiple Lidar sensors positioned around the machine create a point cloud to monitor the environment and ensure safe operation.
- **Isaac Sim Integration**: Used for virtual simulation of physical setups, tool sizes, and materials, with plans for future VR/AR integration.
- **OpenGL Visualization**: Current system provides 3D simulation, with potential for future integration with VR and AR headsets for immersive experiences.

---

## 🚀 Future Development

- **Material API Integration**: Expand material properties API to automatically update and improve material-based operations.
- **Enhanced VR/AR Interfaces**: Integrate AR/VR for real-time monitoring and control of CNC machines.
- **AI Training Improvements**: Further refine the AI model for better handling of more complex machining scenarios and advanced materials like titanium and ceramics.
- **Simulation in Microgravity**: Experiment with environments where gravity is absent for specialized machining use cases.

---

## 🎯 Goals

- ✅ Implement real-time conversion of sensor data to G-code.
- ✅ Deploy unsupervised machine learning model on Google Coral TPU.
- ✅ Integrate system with CNC machine for live operation.
- 🔄 Develop advanced safety mechanisms based on AI predictions and material properties.
- 🔄 Implement augmented reality and virtual reality interfaces for enhanced user interaction and monitoring.

---

## 🌟 Getting Started

To contribute or get started with this project:

1. Clone this repository to your local machine.
2. Follow the setup and configuration instructions to prepare your hardware.
3. Review the documentation and code comments for an overview of the system architecture and operation.
4. Experiment with the system using your CNC machine and observe the enhancements in operation and safety.

---

## 💡 Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Submit a pull request with a comprehensive description of changes.

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 📬 Contact

For inquiries or contributions, please contact us at [dkohlkatl@gmail.com](mailto:dkohlkatl@gmail.com).

