# Nexus-vr[project_readme.md](https://github.com/user-attachments/files/34163650/project_readme.md)
# 🎮 NexusVR - Next-Gen PCVR Remote Streaming & Control Dashboard

![NexusVR Banner](https://img.shields.io/badge/NexusVR-v3.4_PRO-00f0ff?style=for-the-badge&logo=virtualreality&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Meta_Quest_|_Pico_|_PCVR_|_WebXR-7000ff?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-00ff88?style=for-the-badge)

**NexusVR** is a low-latency, specs-agnostic PCVR streaming and remote desktop management interface designed to deliver Virtual Desktop-grade PCVR streaming across high-end gaming rigs and low-spec laptops alike. 

Featuring host-side zero-copy memory pipelines, dynamic bitrate adjustments, integrated AMD FSR spatial upscaling, direct IP headset pairing, and real-time controller telemetry diagnostics, NexusVR turns any browser-enabled device into a PCVR streaming hub.

---

## ✨ Key Features

- ⚡ **Low-Spec Hardware Agnostic Engine:** Optimized algorithms with dynamic pixel reduction and FSR (FidelityFX Super Resolution) support to allow low-end host PCs and laptops to stream smoothly.
- 📡 **Dual Connection & Direct IP Modes:** Support for **Wi-Fi 6E (UDP/WebRTC)** wireless streaming, **USB 3.2 Optical Link** direct tethering, and direct VR headset IP address linking.
- 🎯 **Interactive Controller Input Tester:** Real-time 6-DOF controller telemetry visualization with analog stick tracking, pressure-sensitive trigger/grip meters, and haptic feedback diagnostics.
- 📊 **Real-Time Telemetry & Frame Timing Chart:** Live monitor tracking encode/decode latencies, network jitter, packet loss, and frame drop rates powered by Chart.js.
- 🚀 **PCVR Quick Launcher:** Pre-configured optimization profiles for popular PCVR titles like *Half-Life: Alyx*, *Beat Saber*, *BONELAB*, and *MS Flight Simulator VR*.
- 📲 **VR Client Hub & Pairing:** Built-in IP linking, security PIN pair generation, and WebRTC data connection status indicators.

---

## 🛠️ Architecture & Tech Stack

The dashboard is built as an ultra-compact single-file web interface utilizing modern front-end technologies:

* **Markup & UI:** HTML5 & Tailwind CSS (Custom Cyberpunk / Glassmorphic styling)
* **Icons:** [Lucide Icons](https://lucide.dev/)
* **Analytics & Graphs:** [Chart.js](https://www.chartjs.org/)
* **Audio Synthesizer:** Native Web Audio API for UI sound effects and haptic pulses
* **Graphics Rendering:** HTML5 Canvas API for remote viewport rendering

---

## 🚀 Quick Start Guide

### 1. Running the Control Center
1. Simply clone or download the repository.
2. Open `index.html` in any web browser (Chrome, Edge, Firefox, or Brave). No server setup is required to run the control panel.

### 2. Connecting to Your VR Headset (Meta Quest 2 / 3 / Pro, Pico 4)

1. **Host Setup:** Launch the NexusVR Control Center on your host PC/Laptop (`index.html`).
2. **Direct IP Linking:** Enter your headset's local IP address (e.g. `192.168.1.142`) in the **HEADSET CLIENT PAIRING** section and click **LINK**, or use the **Auto-Detect** feature.
3. **Launch in VR:** On your VR headset client app, enter the 6-digit Security PIN displayed on your PC control dashboard to finish pairing.

---

## 🎛️ Performance Presets

| Mode | Target Framerate | Target Bitrate | Upscaling | Best For |
| :--- | :--- | :--- | :--- | :--- |
| **Ultra Low Spec** | 60 FPS | 45 Mbps | FSR Enabled (70% Scale) | Integrated GPUs, older dual-core CPUs, Wi-Fi 5 |
| **Balanced** | 90 FPS | 95 Mbps | Native 100% | GTX 1660 / RTX 2060+, Wi-Fi 6 |
| **Ultra Graphics** | 120 FPS | 160 Mbps | Supersampled (130% Scale) | RTX 3080 / 4080+, USB 3.2 Link / Wi-Fi 6E |

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
