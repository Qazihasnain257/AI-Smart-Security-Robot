# 🤖 Autonomous AI Smart Security Robot (Work in Progress)

An experimental, edge-computing autonomous surveillance robot designed for low-cost indoor security execution. The project bridges localized microcontroller hardware control loops with high-level Python AI vision analytics over an asynchronous local network.

## 🏗️ System Architecture & Workflow
The system architecture splits processing tasks efficiently across layers to manage hardware resource constraints:

*   **Edge Visual Capture:** An **ESP32-CAM module** acts as the optical edge device, processing low-latency live video frames and streaming the data asynchronously over a local Wi-Fi loop.
*   **Central AI Processing Host:** A remote host machine runs a **Python + OpenCV framework** to ingest the visual telemetry stream and execute real-time person classification and target tracking.
*   **Localized Hardware Automation:** An **Arduino microcontroller** acts as the mechanical execution layer, handling real-time sensory data fusion via an **HC-SR04 ultrasonic array** for autonomous path adjustments while driving DC gear motors via an **L298N H-Bridge driver**.

---

## 🛠️ Project Development Roadmap & Milestones
- [x] Mechanical hardware layout definition and chassis structural configuration.
- [x] Embedded firmware deployment for localized sensor-fusion and L298N motor loops.
- [x] Baseline ESP32-CAM asynchronous HTTP video streaming protocol configurations.
- [ ] Optimization of host-side Python/OpenCV target detection latency matrices (In Progress).
- [ ] Integration of a real-time full-stack network dashboard for remote manual overrides.
- [ ] Final field benchmarking, power calibration, and target latency testing.

---

## 🚀 Future Scope & Full-Stack IoT Expansion
The next major iteration involves constructing a centralized **Node.js and WebSocket backend**. This server architecture will securely ingest multi-threaded data logs, process localized alarm indicators, and serve an interactive full-stack HTML/CSS dashboard for live cross-platform monitoring and remote vehicular control.


